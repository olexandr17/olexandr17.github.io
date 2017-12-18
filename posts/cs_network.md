[Main](/index.md)

## C#. Доступ к сети

Пару часов промучился с проблемой, когда приложение не могло получить доступ к сети, хотя браузер ссылку открывал нормально и флеш с этой ссылкой тоже работал корректно.


Проблема оказалась в том, что программа использовала не дефолтный прокси-сервер.


Теперь о решении проблемы. В каталоге проекта на C# есть шаблонный файл `App.config`, который после компиляции проекта копируется в каталог с бинарником программы под аналогичным именем [AppName].config. Так вот, оказалось, что достаточно добавить в этот конфиг следующие строки:

	
    <?xml version="1.0" encoding="utf-8" ?>
	<configuration>
		<system.net>
			<defaultProxy useDefaultCredentials="true" />
		</system.net>
	</configuration>


p.s. Узелок на память