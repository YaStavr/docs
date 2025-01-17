{% list tabs %}

- Консоль управления

	1. В [консоли управления]({{ link-console-main }}) выберите каталог, в котором находится реестр.
	1. Выберите сервис **{{ iot-short-name }}**.
	1. Выберите реестр.
	1. Перейдите на вкладку **Устройства**.

- CLI
  
	{% include [cli-install](../cli-install.md) %}

	{% include [default-catalogue](../default-catalogue.md) %}

	Получите список устройств в реестре:

	```
	yc iot device list --registry-name my-registry
	```

	Результат:
	
	```
	+----------------------+-----------+
	|          ID          |   NAME    |
	+----------------------+-----------+
	| b9135goeh1uc1s2i07nm | my-device |
	+----------------------+-----------+
	```

- API

    Чтобы получить список устройств в реестре, воспользуйтесь методом REST API [list](../../iot-core/api-ref/Device/list.md) для ресурса [Device](../../iot-core/api-ref/Device/index.md) или вызовом gRPC API [DeviceService/List](../../iot-core/api-ref/grpc/device_service.md#List).

{% endlist %}