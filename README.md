# Warning Email To Employee For Poor Performance

Professional email template for notifying an employee about poor performance

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Professional Services
- **Message Type:** System Notification
- **Tags:** performance review, employee feedback

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/warning-email-to-employee-for-poor-performance.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/warning-email-to-employee-for-poor-performance/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.warning-email-to-employee-for-poor-performance',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
