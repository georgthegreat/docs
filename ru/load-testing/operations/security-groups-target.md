# Настройка групп безопасности цели тестирования

{% include [security-groups-note](../../_includes/vpc/security-groups-note-services.md) %}

{% include [security-groups-target](../../_includes/load-testing/security-groups-target.md) %}

{% note info %}

Вы можете задать более детальные правила для групп безопасности, например, разрешающие трафик только в определенных подсетях.

Важно, чтобы группы безопасности были корректно настроены для всех подсетей, в которых будут размещены цели тестирования.

{% endnote %}