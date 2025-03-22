# 🚀 Zabbix Agent 2 Kurulum ve Yapılandırma

Bu Ansible Playbook, **Zabbix Agent 2**'yi otomatik olarak yükler, yapılandırır ve başlatır. 🖥️  

## 📌 Kullanım  
1. Ansible yüklü olduğundan emin ol.  
2. `inventory.ini` dosyanı oluştur ve Zabbix agent makinelerini ekle.

Örnek kullanım;
```sh
[agents]
CT103 ansible_host=192.168.233.153 ansible_user=root
CT104 ansible_host=192.168.233.154 ansible_user=root
```


4. Aşağıdaki komutu çalıştır:  

   ```sh
   ansible-playbook -i inventory zabbix-agent2.yml
    ```

## 🔧 Neler Yapıyor?  
✔️ Gerekli bağımlılıkları yüklüyor.  
✔️ Zabbix deposunu ekliyor.  
✔️ Zabbix Agent 2'yi kuruyor ve yapılandırıyor.  
✔️ Servisi etkinleştirip yeniden başlatıyor.  
   
