# jj-file
thinkphp 上的网友"将军"写的 file class

## 演示

     //创建目录
     File::mk_dir($dir);
     //读取文件内容
     File::read_file($filename);
     //文件写入
     File::write_file($filename,$content,$openmod);
     //目录删除
     File::del_dir($dir);
     //复制目录
     File::copy_dir($surDir,$toDir);
     //列出目录
     $dirArray = File::get_dirs($dir);
     //$dirArray['dir']:存文件夹；$dirArray['file']：存文件
     //统计文件夹大小,单位 B
     File::get_size($dir);
     //检测是否为空文件夹
     if(File::empty_dir($dir)==true)
     {
        echo $dir.'不是空文件夹';
     }
     //文件缓存与文件读取
     File::cache($name, $value='', $path=DATA_PATH,$cached=true) ;

via: http://www.thinkphp.cn/extend/436.html
