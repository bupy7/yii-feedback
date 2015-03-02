Yii-Feedback
============

Yii-Feedback - this is extension for send email from Yii. This modification extension YiiFeedbackWidget https://github.com/gazbond/YiiFeedbackWidget.

### Required

- YiiBooster 3.0.1 https://github.com/clevertech/YiiBooster/tree/3.0.1

### Install
Install YiiBooster https://github.com/clevertech/YiiBooster/blob/3.0.1/INSTALL.md

Download or clone the files from repository https://github.com/PHPMailer/PHPMailer to your extensions directory:
```
[app-root]/protected/extensions/phpmailer/
```

Download or clone the files to your extensions directory:
```
[app-root]/protected/extensions/feedback/
```
Add in your view follow code:
```php
$this->widget(
    'ext.feedback.FeedbackWidget', 
    array(
        'topicOptions' => array(
            'first_topic',
            'second_topic',
            'third_topic',
        ),
        'toEmail' => 'your@email.com',
        'title' => 'Title feedback',
    )
);
```

### Changes
###### Added:
+ Rewrited with using Yii-booster.
+ Support PHPMailer.
+ Russian language.
+ Transition to anchor after send mail.
+ "title" in config options for feedback form.

###### Removed:
+ "position" from config options.
