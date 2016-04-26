Digital Direct IVR
==================
Digital Direct api voice

[![Latest Stable Version](https://poser.pugx.org/ignatenkovnikita/yii2-digitaldirect-ivr/v/stable)](https://packagist.org/packages/ignatenkovnikita/yii2-digitaldirect-ivr) [![Total Downloads](https://poser.pugx.org/ignatenkovnikita/yii2-digitaldirect-ivr/downloads)](https://packagist.org/packages/ignatenkovnikita/yii2-digitaldirect-ivr) [![Latest Unstable Version](https://poser.pugx.org/ignatenkovnikita/yii2-digitaldirect-ivr/v/unstable)](https://packagist.org/packages/ignatenkovnikita/yii2-digitaldirect-ivr) [![License](https://poser.pugx.org/ignatenkovnikita/yii2-digitaldirect-ivr/license)](https://packagist.org/packages/ignatenkovnikita/yii2-digitaldirect-ivr)

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist ignatenkovnikita/yii2-digitaldirect-ivr "*"
```

or add

```
"ignatenkovnikita/yii2-digitaldirect-ivr": "*"
```

to the require section of your `composer.json` file.

Usage
-----

Add this to your main configuration's components array:

```php
'ivr' => [
            'class' => \ignatenkovnikita\digitaldirectivr\ClientVoice::className() ,
            'url' => 'https://api.digital-direct.ru',
            'login' => 'your_login',
            'pass' => 'your_password'
        ],
```
Typical component usage
-----------------------
```php
Yii::$app->ivr->statusOneMessage(id);
Yii::$app->ivr->sendMessage(params);
```


