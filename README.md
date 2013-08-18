jalali-fullcalendar
===================

Jalali FullCalendar

Great JavaScript calendar converted to Yii extension.

Example usage:
```php
<?php 
$this->widget('ext.JFullCalendar.JFullCalendar', array(
    'options'=>array(
        'header'=>array(
            'left'=>'prev,next',
            'center'=>'title',
            'right'=>'today'
        )
    )));
?>
```

sample load event from  controller:
```php
'events'=>$this->createUrl('event/calendarevents'),
```
and load from two or more controllers:

```php
'eventSources'=>array(
	$this->createUrl('event/calendarevents'),
	$this->createUrl('site/calendarevents'),
),
```
