```php
public function calculateScore(User $user): int
{
    if ($user->inactive) {
        return 0;
    }

    if ($user->hasBonus) {
        return $user->score + $this->bonus;
    }

    return $user->score;
}
```
