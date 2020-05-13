```js
<!-- HTML -->
<el-scrollbar class="scroll" view-class="scroll-view"></el-scrollbar>

<!-- CSS -->
.scroll {
    width: $scroll-w; 
    height: $scroll-h;
    
    // 修正横向滚动条问题
    ::v-deep .el-scrollbar__wrap {
        overflow-x: hidden; 
    }
    
    // 添加 view “左右”内边距
    ::v-deep .scroll-view {
        padding: 0 15px;
    }
    
    // 添加 view “上下”内边距
    padding: 15px 0;
}

注意：尺寸是百分比时，需要保证父有确切的尺寸！！
```

