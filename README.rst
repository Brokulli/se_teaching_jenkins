Jenkins
=======

1. Uruchom jenkins-a:

   ::

     make build_jenkins
     make run_jenkins

    ::

    jesli nie dziala to wykonujemy na root
    (linie 107-114 z se_teaching_vm_images/vagrant/centos/Vagrantfile)

    yum install -y yum-utils
        yum-config-manager \
           --add-repo \
           https://download.docker.com/linux/centos/docker-ce.repo
        yum makecache fast
        yum install docker-ce -y
        systemctl start docker && \

2. Następnie otwórz w przeglądarce 127.0.0.1:8080,
jeśli zostaniesz poproszony o hasło dla admina, na root wpisz poniższą komendę
i  wklej haslo (tu: eeba707d659f48258aa0b770fa394882):

   ::

     cat jenkins/secrets/initialAdminPassword


3. Wybierz *Suggested plugins* // instalacja sugerowanych wtyczek


4. Kontunuuj jako administrator

  ::

    hasło: jak powyżej
    login: admin
    

Related
-------

- https://github.com/sheehan/job-dsl-gradle-example
