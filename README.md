# EFK стек

Включає:

- Elasticsearch
- Fluentd
- Kibana


## Запуск EFK стеку

### Вимоги

На вашій машині, повнні бути встановлені:

- Docker
- Docker Compose
- Node.js


### Запуск

```bash
docker-compose up
```

Зверніть увагу: Fluentd запущений на порту `24224`.

Kibana відкрита на порту `5601`.

Тоді відвідайте http://localhost:5601/ у своєму браузері.

Налаштуйте шаблон імені індексу `fluentd-*`. 

Потім перейдіть на `Discover` вкладку, щоб знайти журнали.

### Застосунок

Запустіть `npm init -y` і вставте наступне в index.js.

Встановіть логгер командою  `npm install fluent-logger` та запустыть застосунок `node index.js`.