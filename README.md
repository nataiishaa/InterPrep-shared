# InterPrep-shared

Общие Proto-контракты для бэкенда и клиентов (iOS InterPrep и др.).

## Структура

- **proto/** — файлы `.proto` (auth, user, gateway, calendar, materials, coach, jobs, common).

## Использование

- **Go (бэкенд):** `protoc` с `--go_out`, `--go-grpc_out`.
- **Swift (iOS):** `protoc` с плагином `swift-protobuf`; в proto указан `option swift_prefix` для имён типов.

Импорт `google/protobuf/timestamp.proto` в calendar — стандартный, при генерации нужен путь к `google/protobuf` (обычно идёт с установкой protoc).

## Репозиторий

```
git@github.com:nataiishaa/InterPrep-shared.git
```
