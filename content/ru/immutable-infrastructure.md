---
title: Неизменяемая инфраструктура
status: Completed
category: property
tags: ["infrastructure", "property", ""]
---

Неизменяемая инфраструктура — это компьютерная инфраструктура 
([виртуальные машины](/virtual-machine/), [контейнеры](/ru/container/), сетевые устройства), 
которую невозможно изменить после развертывания. 
Неизменяемость может быть реализована с помощью автоматического процесса, который перезаписывает несанкционированные изменения, или 
с помощью системы, которая вообще не позволяет вносить изменения. 
Контейнеры — хороший пример неизменяемой инфраструктуры. 
Внести в них постоянные изменения можно, только  
создав новую версию контейнера или воссоздав существующий контейнер из его образа.

Предотвращая или выявляя несанкционированные изменения, 
неизменяемые инфраструктуры облегчают обнаружение и предотвращение угроз безопасности. 
Управлять такой системой гораздо проще, 
поскольку администраторам легче предугадывать её поведение. 
Ведь они знают, что никто не мог внести в нее изменения (в т.ч. ошибочные), о которых, к тому же, забыл сообщить. 
Неизменяемая инфраструктура неразрывно связана с подходом [«инфраструктура как код»](/ru/infrastructure-as-code/) 
при котором вся автоматизация, необходимая для создания инфраструктуры, хранится в системе контроля версий (например, Git). 
Такое сочетание неизменяемости и контроля версий позволяет 
вести долговременный журнал аудита каждого авторизованного изменения в системе.
