# interaction_design
1.target="_blank"可以在新的页面打开网页

2.网页标题的改动
  <script>
        document.addEventListener("visibilitychange", function () {
            if (document.visibilityState === 'hidden') {
                document.title = '你找不到我';
            } else {
                document.title = '啊哈被你找到了';
                    setTimeout(function () {
                        document.title = 'My Web Page';
                    }, 2000); // 两秒钟后恢复原标题
            }
        });
        
    </script>
