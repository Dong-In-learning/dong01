<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Flex</title>
    <style>
      body {
        margin: 0;
        height: 100vh;
        background-color: #eee;
      }
      /* * {
        border: 1px solid black;
      } */

      .flex {
        display: flex;
      }

      .column {
        flex-direction: column;
      }

      .flex1 {
        flex: 1;
      }

      .baiSe {
        background-color: white;
      }

      .daoHang {
        padding: 10px 20px;
        border-bottom: 1px solid rgb(190, 190, 190);
        font-size: 14px;
        counter-reset: #666;
      }

      .yinYing {
        box-shadow: rgb(0 0 0 / 20%) 0px 2px 1px -1px,
          rgb(0 0 0 / 14%) 0px 1px 1px 0px, rgb(0 0 0 / 12%) 0px 1px 3px 0px;
      }

      .mg8 {
        margin: 8px;
      }

      .mgr8 {
        margin-right: 8px;
      }

      .mgt8 {
        margin-top: 8px;
      }
    </style>
  </head>
  <body class="flex">
    <!-- 侧边栏 -->
    <div class="baiSe yinYing" style="width: 200px">
      <!-- 头像 -->
      <div
        style="
          padding: 10px;
          align-items: center;
          justify-content: center;
          border-bottom: 1px solid #999;
        "
        class="flex"
      >
        <img src="image/head.webp" width="40px" height="40px" alt="" />
        <div style="margin-left: 10px">东</div>
      </div>
      <!-- 导航栏 -->
      <div class="flex column">
        <div class="daoHang">导航</div>
        <div class="daoHang">导航</div>
        <div class="daoHang">导航</div>
        <div class="daoHang">导航</div>
        <div class="daoHang">导航</div>
        <div class="daoHang">导航</div>
      </div>
    </div>
    <!-- 主区域 -->
    <div class="flex flex1 column">
      <!-- 头部栏 -->
      <div style="height: 60px; z-index: 1" class="baiSe yinYing"></div>
      <!-- 内容区 -->
      <div style="overflow: auto" class="flex flex1 mg8">
        <!-- 左区 -->
        <div style="flex: 3" class="flex column">
          <!-- 数据区 -->
          <div class="flex">
            <!-- 数据块 -->
            <div style="height: 100px" class="flex1 baiSe yinYing mgr8"></div>
            <div style="height: 100px" class="flex1 baiSe yinYing mgr8"></div>
            <div style="height: 100px" class="flex1 baiSe yinYing mgr8"></div>
            <div style="height: 100px" class="flex1 baiSe yinYing mgr8"></div>
          </div>
          <!-- 列表区 -->
          <div class="flex column">
            <!-- 列表项 -->
            <div style="height: 160px" class="baiSe yinYing mgt8 mgr8"></div>
            <div style="height: 160px" class="baiSe yinYing mgt8 mgr8"></div>
            <div style="height: 160px" class="baiSe yinYing mgt8 mgr8"></div>
            <div style="height: 160px" class="baiSe yinYing mgt8 mgr8"></div>
            <div style="height: 160px" class="baiSe yinYing mgt8 mgr8"></div>
            <div style="height: 160px" class="baiSe mgt8 mgr8"></div>
          </div>
        </div>
        <!-- 右区 -->
        <div class="flex column mgr8" style="flex: 1">
          <!-- 提示区 -->
          <div style="height: 160px" class="baiSe yinYing"></div>
          <!-- 消息区 -->
          <div style="height: 160px" class="baiSe yinYing mgt8"></div>
        </div>
      </div>
    </div>
  </body>
</html>
