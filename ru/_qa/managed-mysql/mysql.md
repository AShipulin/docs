# Вопросы о {{ MY }}

#### Какие версии {{ MY }} поддерживает {{ mmy-short-name }}? {#supported-version}

{{ mmy-short-name }} поддерживает {{ MY }} 5.7 и {{ MY }} 8.

#### Включено ли резервное копирование кластеров БД по умолчанию? {#backup}

Да, по умолчанию резервное копирование включено. Для {{ MY }}-кластеров выполняется полное резервное копирование один раз в сутки, и сохраняются все журналы транзакций кластера БД. Это позволяет восстановить состояние кластера на любой момент времени в пределах периода хранения резервных копий, за исключением последних 30 секунд.

#### Шифруется ли соединение с кластером БД {{ MY }}? {#encryption}

Соединение между кластером БД и приложением всегда шифруется с использованием SSL. Отключить шифрование соединений с кластером нельзя.

#### Что такое реплика для чтения в {{ MY }}? {#read-only-instance}

Реплика для чтения — это доступный только для чтения хост в кластере БД {{ MY }}, данные на котором синхронизируются с хостом-мастером (если в кластере работает более 1 хоста). Вы можете использовать реплику для чтения для снижения нагрузки на мастер в базах данных с большим объемом запросов на чтение.

#### Какие ограничения накладываются на кластеры БД {{ MY }}? {#instance-limitations}

Подробнее об ограничениях {{ mmy-short-name }} см. раздел [{#T}](../../managed-mysql/concepts/limits.md). В разделе [{#T}](../../managed-mysql/concepts/instance-types.md) приведены характеристики кластеров, которые можно создать с помощью {{ mmy-short-name }}.
