# Версионирование проекта.
### Пример: "version": "1.2.3.42"

MAJOR — крупные изменения (новая глава, новая механика), могут требовать полной переустановки DLC.<br/>
MINOR — новые фичи/уровни, обычно совместимы с текущей базой. <br/>
PATCH — исправления багов, баланс, мелкие правки.<br/>
BUILD — номер сборки, который можно автоинкрементировать при каждом CI/CD-билде, чтобы отличать тестовые сборки.<br/>


# JSon структура файла.
```
{
  "builds": [
    {
      "build_version": "1.0.1.0",
      "Windows" : [
        {
          "Manifest_URL":"Some_URL",
          "Pak_URL":"Some_URL"
        }
      ],
      "Android" : [
       {
          "Manifest_URL":"Some_URL",
          "Pak_URL":"Some_URL"
       }
      ]
    },
    {
      "build_version": "1.0.0.1",
      "Windows" : [
        {
          "Manifest_URL":"Some_URL",
          "Pak_URL":"Some_URL"
        }
      ],
      "Android" : [
       {
          "Manifest_URL":"Some_URL",
          "Pak_URL":"Some_URL"
       }
      ]
    }
  ]
}
```
