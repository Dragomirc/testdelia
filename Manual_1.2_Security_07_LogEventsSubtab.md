---
id: Manual_1.2_Security_07_LogEventsSubtab
title: Log Events Subtab
---

<style>
div.post > article > div > span {
  text-align: justify;
}
</style>


The <label>Log Events / Evenimentele jurnalului / События журнала</label> subtab 
from the <label>Security / Securitate / Безопасность</label> tab contains records 
of error and status messages from all the modules of MOLDLIS, saved as logs. 

From logging messages it is possible to see what the system is doing
without consulting the logs of the servers that host individual modules.
<br>

Figure “The Log Events Subtab” shows the components of the <label>Log Events / Evenimentele jurnalului / События журнала</label> subtab.

![LogEventsSubtab](assets/1.2_Security_LogEventsSubtab.jpg)
<figcaption>“The Log Events Subtab”</figcaption>
<br>

The <label>Log Events / Evenimentele jurnalului / События журнала</label> subtab lists 
the following information about the recorded log messages:


* <label>Time / Ora / Время</label>: Shows the date and time when the message was logged in the format YYYY-MM-DD HH:MM:SS.


* <label>Severity / Severitate / Важность </label>: Shows the severity level of the log message.<br>
The level gives a rough guide to the importance and urgency of a log message:

     * `OFF`	The highest possible rank (this value is intended for turning off logging and should never appear in any real log event messages).

     * `FATAL`	Designates very severe error events that will presumably lead the application to abort.

     * `ERROR`	Designates error events that might still allow the application to continue running.

     * `WARN`	Designates potentially harmful situations.

     * `INFO`	Designates informational messages that highlight the progress of the application at coarse-grained level.

     * `DEBUG`	Designates fine-grained informational events that are most useful to debug an application.

     * `TRACE`	Designates finer-grained informational events than the `DEBUG`.

	 
* <label>Module / Modul / Модуль</label>: Shows the component that emitted the log event record.


* <label>Message / Mesaj / Сообщение</label>: Shows the text payload carrying the actual log message.


* <label>Context / Context / Контекст</label>: Shows the arbitrary data passed with the construction of the message, for example, `RequestID=347d2742-4348-4382-8087-c20de52e1677, Module=AAC`.


* <label>Other / Altele / Другой</label>: Shows auxiliary information about the log event record, such as the details of the server, process and code where the record was produced.
