jalali-fullcalendar
===================

Jalali FullCalendar  

[![Latest Stable Version](https://poser.pugx.org/faravaghi/jalali-fullcalendar/v/stable)](https://packagist.org/packages/faravaghi/jalali-fullcalendar) [![Total Downloads](https://poser.pugx.org/faravaghi/jalali-fullcalendar/downloads)](https://packagist.org/packages/faravaghi/jalali-fullcalendar) [![Latest Unstable Version](https://poser.pugx.org/faravaghi/jalali-fullcalendar/v/unstable)](https://packagist.org/packages/faravaghi/jalali-fullcalendar) [![License](https://poser.pugx.org/faravaghi/jalali-fullcalendar/license)](https://packagist.org/packages/faravaghi/jalali-fullcalendar)

Great JavaScript calendar converted to Yii extension with [Full Calendar](http://arshaw.com/fullcalendar/).

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
If you are on Jalai date, need the convert Jalai to Gregorian for show in calendar.
for example if your date is '1392/05/27' , need convert to '2013/08/18'.
