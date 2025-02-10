# Sky Torch天空火炬
## 介绍
此插件是为视频开发的：
[Orbital Laser in Minecraft (Sky Torch)](https://youtu.be/OKXTGbp6AMk)

## 安装
1. 从 [releases page](https://github.com/TheCymaera/minecraft-sky-torch/releases/)下载 JAR。
2. 设置 [Paper](https://papermc.io/downloads) or [Spigot](https://getbukkit.org/download/spigot) 服务器。(说明如下）
3. 将 JAR 添加到 `plugins` 文件夹。
4. 从 [Planet Minecraft](https://www.planetminecraft.com/project/ambertry-forest/)下载世界文件夹。
	- 这是可选项。您可以使用任何喜欢的世界。
5. 将世界文件夹放入服务器目录。将其命名为 `world`。

## 运行服务器
1. 从 [Paper](https://papermc.io/downloads) or [Spigot](https://getbukkit.org/download/spigot)下载服务器 JAR。
2. 运行以下命令 `java -Xmx1024M -Xms1024M -jar server.jar nogui`。
3. 我通常使用与 Minecraft 安装捆绑的 Java 运行时，以避免版本冲突。
   - 在 Modrinth 中，你可以在配置文件选项菜单中找到 Java 运行时的位置。
4. 将`eula.txt`文件中的`eula=false`改为`eula=true`，接受 EULA。
5. 以 `localhost` 作为 IP 地址加入服务器。


## 命令
自动完成将显示可用选项。
```
# 获取控制物品
/items

# 加载选项预设
/preset <preset:enum>

# 重载选项（手动编辑配置文件后）
/reload_config

# 更改激光尺度
/scale <scale:double>
```

## Development
1. Clone or download the repo.
2. Run Maven `package` to build the plugin. The resulting JAR will be in the `target` folder.
3. For convenience, set up a symlink and add the link to the server `plugins` folder.
   - Windows: `mklink /D newFile.jar originalFile.jar`
   - Mac/Linux: `ln -s originalFile.jar newFile.jar `

## License
You may use the plugin and source code for both commercial or non-commercial purposes.

Attribution is appreciated but not due.

Do not resell without making substantial changes.
