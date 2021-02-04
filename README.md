# es_docker_compose
使用 docker-compose，建立的 ES Docker Container<br>

# 說明
docker-compose 檔案內有設定 Container 可使用的 CPU 與 Memory 上限，另有 Port 對應功能<br>
ES 建立時會消耗不少記憶體，在剛建立時，就會消耗近 6 GB 的記憶體，請依照需求調整記憶體<br>
Container 建立後，會使用 volumes 映射資料夾（./es/data/:/usr/share/elasticsearch/data），即使 Container 因為任何意外移除或故障，重啟或重新建立後，資料也不會遺失。
