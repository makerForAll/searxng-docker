## 启动项目

在成功创建并配置好 `docker-compose.yml` 和 `data/settings.yml` 文件后，您可以使用以下命令启动 SearXNG 项目：

1. **打开终端**，导航到项目目录：
   ```bash
   cd /path/to/your/searxng
   ```

2. **启动 Docker 服务**：
   ```bash
   docker-compose up -d
   ```

   这条命令会在后台启动 SearXNG 服务。

3. **检查服务状态**：
   您可以使用以下命令查看服务的运行状态和日志：
   ```bash
   docker-compose logs -f
   ```

4. **访问 SearXNG**：
   在浏览器中打开以下地址：
   ```
   http://localhost:8080
   ```

   现在您可以在搜索框中输入关键词并点击搜索按钮，开始使用 SearXNG。

5. **停止服务**：
   如果您需要停止 SearXNG 服务，可以使用以下命令：
   ```bash
   docker-compose down
   ```

   这将停止并删除所有相关的 Docker 容器。


    get请求
   http://localhost:8080/search?q={内容}&format=json