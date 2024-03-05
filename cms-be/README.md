## 安装与运行

项目运行之前，请确保系统已经安装以下应用

- node (6.0 及以上版本)
- mongodb (开启状态)

运行命令

```
git clone git@github.com:lzc1220/background_management_system.git
cd background_management_system/cms-be

npm install

#development
npm run dev

#production
npm run build

# 批量导入测试数据
# 见 脚本 part
```

## 脚本

为了方便开发测试，提供下列脚本

```
# 自动导入测试数据
npm run import

# 移除多余文件
npm run clean

# 给丢失头像的学生分配默认头像
npm run default

# 把目录下的md移动到src/file/md
npm run rm
```

## 技术特点

- Koa
- TypeScript
- cookie-session 鉴权(普通请求) + jwt 鉴权(img 标签的 src，携带 token)

## 其它

见本目录下的'实现细节.md'
