# Версионирование проекта.
### Пример: "version": "1.2.3.42"

MAJOR — крупные изменения (новая глава, новая механика), могут требовать полной переустановки DLC.<br/>
MINOR — новые фичи/уровни, обычно совместимы с текущей базой. <br/>
PATCH — исправления багов, баланс, мелкие правки.<br/>
BUILD — номер сборки, который можно автоинкрементировать при каждом CI/CD-билде, чтобы отличать тестовые сборки.<br/>


# JSon структура файла.
```
{
  "deploy_timestamp": "2025-11-06T12:00:00Z",
  "builds": [
    {
      "build_id": 450,
      "required_base_build": 448,
      "dlc_information": [
        {
          "chunk_id": "Content_Chunk",
          "platform_data": {
            "Windows": {
              "file_pairs": {
                "https://cdn.example.com/win/Man_A.json": "https://cdn.example.com/win/Pak_A.pak",
                "https://cdn.example.com/win/Man_B.json": "https://cdn.example.com/win/Pak_B.pak"
              }
            },
            "Android": {
              "file_pairs": {
                "https://cdn.example.com/android/Man_A.json": "https://cdn.example.com/android/Pak_A.obb",
                "https://cdn.example.com/android/Man_B.json": "https://cdn.example.com/android/Pak_B.obb"
              }
            }
          }
        }
      ]
    },
    {
      "build_id": 452,
      "required_base_build": 450,
      "dlc_information": [
        {
          "chunk_id": "Content_Chunk",
          "platform_data": {
            "Windows": {
              "file_pairs": {
                "https://cdn.example.com/win/Man_A.json": "https://cdn.example.com/win/Pak_A.pak",
                "https://cdn.example.com/win/Man_B.json": "https://cdn.example.com/win/Pak_B.pak"
              }
            },
            "Android": {
              "file_pairs": {
                "https://cdn.example.com/android/Man_A.json": "https://cdn.example.com/android/Pak_A.obb",
                "https://cdn.example.com/android/Man_B.json": "https://cdn.example.com/android/Pak_B.obb"
              }
            }
          }
        }
      ]
    }
  ]
}
```
