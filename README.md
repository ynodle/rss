hexo资源优化

1.hexo-neat
npm install hexo-neat --save

项目配置文件下添加
# hexo-neat
# 博文压缩
neat_enable: true
# 压缩html
neat_html:
  enable: true
  exclude:
# 压缩css  
neat_css:
  enable: true
  exclude:
    - '**/*.min.css'
# 压缩js
neat_js:
  enable: true
  mangle: true
  output:
  compress:
  exclude:
    - '**/*.min.js'
    - '**/jquery.fancybox.pack.js'
    - '**/index.js' 

2. gulp
sudo npm install --global gulp --unsafe-perm
npm install gulp-minify-html gulp-minify-css gulp-uglify gulp-imagemin
npm install gulp-terser --save-devclear
项目根目录添加gulpfile.js
