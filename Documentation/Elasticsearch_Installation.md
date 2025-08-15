In this demo, I follow the official Elastic documentation as a reference.
https://www.elastic.co/docs/solutions/search/get-started

Choose Elasticsearch depending on your server's architecture and platform and copy the link download URL on Elastic official website. https://www.elastic.co/downloads/elasticsearch

<img src="https://github.com/user-attachments/assets/dbb8f003-7a7f-4960-bb22-66c59bb8d467" />

### 1. Download Elasticsearch using **wget** 
```
wget -O https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-9.1.2-amd64.deb
```
Once downloaded, you will see the .deb file in your downloaded directory.

<img width="1159" height="299" alt="2" src="https://github.com/user-attachments/assets/b8c95a48-1b35-434a-9609-7f9db9c9f0f7" />

### 2. Install Elasticsearch debian package using **dpkg** installer

```
dpkg -i elasticsearch_package_name.deb
```

After extracting and installing the elasticsearch package, you will be presented with elastic built-in superuser credentials. Make sure to save it for future use.

<img width="1177" height="732" alt="3" src="https://github.com/user-attachments/assets/9b47f5b7-d867-4b89-b93c-28bc8194e50b" />

### 3. Configure Elasticsearch.yml file

Elasticsearch configuration files are located in /etc/elastichsearch directory. Use `nano` or `any text editor you like` to configure elasticsearch.yml file.

<img width="1171" height="163" alt="4" src="https://github.com/user-attachments/assets/c1fbd953-5b15-458e-8425-e3b9823a9cb7" />

In the Network configuration, uncomment the network host and set your ip, port according to your environment. (Default port number for elasticsearch is 9200)

<img width="826" height="273" alt="5" src="https://github.com/user-attachments/assets/6eb76e89-de31-4914-a3e6-9c53e2823547" />

Once you've modified the elasticsearch.yml configuration file, enable and start the elasticsearch.service.
```
systemctl enable elasticsearch.service
systemctl start elasticsearch.service
```
<img width="1178" height="406" alt="6" src="https://github.com/user-attachments/assets/245861ec-99ce-4249-8974-28d3e8e1f7d7" />
