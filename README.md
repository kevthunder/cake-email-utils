## Usage

```php
    //var $components = array('Email','EmailUtils');
    $conf = array(
      'subject' => __('Subject',true),
      'to' => 'email@server.com',
      'sender' => $this->EmailUtils->defaultEmail(),
      'replyTo' => null,
      'sendAs' => 'both', // because we like to send pretty mail
      'template' => 'template',
      'layout' => null
    );
    $this->EmailUtils->setConfig($conf);

    $this->EmailUtils->set('var', $var);

    if(!$this->Email->send()){
      
    }else{
      
    }
```