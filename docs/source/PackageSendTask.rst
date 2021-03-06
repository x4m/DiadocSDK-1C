﻿PackageSendTask
===============

Объект предназначен для отправки сообщения с пакетом документов на сервер Диадок.

Свойства
--------

-  **Content** (чтение/запись) - содержание пакета документов, имеет тип 
   :doc:`SentPackageContent <SentPackageContent>`
-  **OperationId** (строка, чтение/запись) - уникальный идентификатор
   операции
-  **CounterAgentId** (строка, чтение/запись) - идентификатор контрагента
-  **FromDepartmentId** (строка, чтение/запись) - идентификатор
   подразделения отправителя
-  **ToDepartmentId** (строка, чтение/запись) - идентификатор подразделения
   получателя
-  **IsDraft** (булево, чтение/запись) - признак того, что сообщение является
   черновиком
-  **IsInternal** (булево, чтение/запись) - признак того, что сообщение
   является внутренним, то есть сообщением между подразделениями
   организации
-  **LockPackage** (булево, чтение/запись) - признак того, что пакет после
   отправки должен быть нередактируемым
-  **DelaySend** (булево, чтение/запись) - признак того, что сообщение будет
   сохранено без отправки
-  **DocumentsToSend** (:doc:`коллекция <Collection>` объектов :doc:`DocumentToSend <DocumentToSend>`, чтение) -
   коллекция документов, уже добавленных в пакет


Методы
------

-  :doc:`AddDocument <AddDocument>` - добавляет документ заданного типа
   в пакет на отправку
-  :doc:`AddDocumentFromFile <AddDocumentFromFile>` - добавляет документ 
   в пакет на отправку, загружая его из файла
-  :doc:`Send <Send-(PackageSendTask)>` - отправляет пакет документов на сервер
-  :doc:`SendAsync <SendAsync-(PackageSendTask)>` - инициирует асинхронную отправку 
   пакета документов

.. toctree::
   :name: Auto
   :hidden:

   AddDocument <AddDocument>
   AddDocumentFromFile <AddDocumentFromFile>
   Send <Send-(PackageSendTask)>
   SendAsync <SendAsync-(PackageSendTask)
