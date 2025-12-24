# lab_ansible_roles #6
1. Была создана role, которая устанавлиявает nginx с vhosts

   а) Прописывается первая задача в ./roles/nginx-vhosts/tasks/main.yml по установке NGINX на хост. В качестве второй задачи: копирование в цикле конфигурации для ВМ.

   б) Затем создаются файлы site.conf.j2 и index.html.j2 с данными о страницах виртуального сайта

   в) Отдельно создается скрипт run_playbook.sh, который помогает запускать плейбук к ролью

2.  Прогон плейбука

    <img width="813" height="575" alt="image" src="https://github.com/user-attachments/assets/4c94b81f-e64a-4aae-9342-df044abf56f2" />

3. Проверка с командной сроки указанем HTTP заголовок host

   <img width="603" height="407" alt="image" src="https://github.com/user-attachments/assets/d3449d07-248c-4dc2-8e7a-81824dd1adea" />

4. Обманываем чуть-чуть DNS, поправляя файл hosts, и заходим на сайт etis.com

   <img width="847" height="286" alt="image" src="https://github.com/user-attachments/assets/655e079c-381f-4264-a86f-b3b69c966334" />

5. Правим /etc/hosts и проверяем через lynx по имени сайта

   <img width="426" height="125" alt="image" src="https://github.com/user-attachments/assets/3fffc810-b072-4855-a2eb-f4b207d6d392" />
   <img width="565" height="131" alt="image" src="https://github.com/user-attachments/assets/fe26c4eb-1fa8-4d13-9edc-aaed669d271a" />

6. Создаем репозиторий lab_ansible_roles

   <img width="1080" height="298" alt="image" src="https://github.com/user-attachments/assets/b8036053-d256-4890-aba9-3b99a55cca55" />

   С помощью git clone git@github.com:catherinezybareva/lab_ansible_roles.git

7. Активируем CI-пайплайны (сценарии)

   <img width="1280" height="737" alt="image" src="https://github.com/user-attachments/assets/a9e59fce-908a-45af-a8a8-a3e0f85ebfdd" />

8. Добавляем сценарий devops_course_pipeline.yml и добавляем сценарии CI в гит

   <img width="777" height="422" alt="image" src="https://github.com/user-attachments/assets/90dc0894-ebc4-4027-ae2e-169466d0c3e6" />

   <img width="890" height="525" alt="image" src="https://github.com/user-attachments/assets/46158377-3a87-4105-b397-1284cb4eb4d2" />

9. Потом добавляем новый "боевой" сценарий lint.yml и просматриваем, как он отрабатывает

    <img width="1280" height="636" alt="image" src="https://github.com/user-attachments/assets/7b6a678f-f100-43f1-b9cf-2a14167e9307" />
