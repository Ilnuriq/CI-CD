# CI/CD. Семинар 4. Troubleshooting (диагностика и решение проблем в CI/CD)


## Решение
Создан локальный файл `local-smoke-tests.gitlab-ci.yml`

```yaml
smoke-test-job:
  script: echo "SMOKE"
```

Создан основной файл `.gitlab-ci.yml`

```yaml
include:
  - local: local-smoke-tests.gitlab-ci.yml
#  - remote: https://github.com/Ilnuriq/CI-CD-4/blob/main/remote_included-file.yml
```




Repository Seminar04
![repository](https://github.com/Ilnuriq/CI-CD-4/blob/main/img/VirtualBox_cibox_47.png)

Remote included file job
![remote included file job](https://github.com/Ilnuriq/CI-CD-4/blob/main/img/VirtualBox_cibox_01.png)

Pipeline passed
![pipeline passed](https://github.com/Ilnuriq/CI-CD-4/blob/main/img/VirtualBox_cibox_34.png)

