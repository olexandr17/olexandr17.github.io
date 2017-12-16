[Main](/index.md)

## С#. OFPerforceTool

В течении последнего время, в свободное время, делал приложение, которое помогло избавиться от монотонной работы и экономит ежедневно до получаса рабочего времени. Но основным мотиватором был все же интерес :).

У нас на работе ежедневно нужно готовить отчет о всех коммитах в Перфорс, которые были сделаны в течении дня. Для задач, которые были заведены в Джире также необходимо было собирать их описания, имея только ссылки. И если команда днем хорошо поработала и сделала, к примеру, 20 коммитов и 10 из них оказались жировскими, то вечером человеку, который готовит отчет, было невесело.

Собственно, описание программы с рабочего Confluence со скриншотами:


__Requirements:__ .NET Framework 4, pre-authorization in Perforce


__1. Merge request__

The purpose of this application is reduction of time, which was spent for making ticket descriptions for MergeRequest.

When you start application first time, it show form with settings.


![_](/img/cs_perforce_tool_1.jpg)


The following fields should be filled or changed:

- Jira URL – Jira URL;
- Jira credentials – your login and password for Jira-account;
- PF work path – our work directory in Perforce;
- PF client – name of your Perforce client;
- PF port – IP and port for Perforce (almost always port in this field should be equal 3530);
- PF days limit – count of previous days during which application will search needed CL;
- Enable responses – debug tool, if checkbox is selected that application will run slower;
- Enable autostart – start application after running your OS.

After filling all settings, you can try to use application :)


![_](/img/cs_perforce_tool_2.jpg)


On main form, you can paste the number of last CL that was included in last MergeRequest and press button “Get information”.

When application receives data, you can copy needed information from corresponding fields. If some CLs weren’t processed properly and application didn’t crash :), in last textfield problem CLs will be shown. These CLs should be processed manually.

Also on main screen of application you can see links for quick access to MR instructions, MR creating and report creating.

__2. Additional tools__

On left side of application there are several buttons:

- Sync – sync work directory in Perforce;
- Force sync – force sync work directory in Perforce;
- Open binaries – reopen your binaries in specified CLs after commit CL;
- Resolve binaries – resolve your binaries with accepting your changes after next sync;

For using last two tools you must fill fields in second tab in Settings Form of correct data.
