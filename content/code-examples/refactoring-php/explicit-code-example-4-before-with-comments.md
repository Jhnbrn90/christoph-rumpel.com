```php
// ❌ We do not care which steps are needed to check for a subscribed user
User::whereNotNull('subscribed')->where('status', 'active');
```