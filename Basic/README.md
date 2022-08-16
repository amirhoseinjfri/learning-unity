**Clamp**

برای استفاده از (clamp) ابتدا باید مثلا از مکان یک جسم یک متغییر موقت بسازید مانند (temPos) سپس تغییرات را روی مقدار موقت انجام داده و سپس تغییرات انجام شده را روی مکان اصلی و فعلی انجام بدهید مانند مثال زیر

```c#
Vector3 tmpPos = transform.position;
tmpPos.x = Mathf.Clamp(tmpPos.x, -2.0f, 2.0f);
transform.position = tmpPos;

OR

transform.position = new Vector3(Mathf.Clamp(transform.position.x, -2.0f, 2.0f), transform.position.y, transform.position.z);
```

**Get Position Direction**

برای اینکه جهت دو نقطه را بدست بیاوریم حتی زاویه را از این دستور استفاده میکنیم
```c#
Vector3 dir = (this.position - one before the last position).normalized;
```

**Snapping Camera or Gameobject to View**

برای چسباندن یا تغییر مکان یک شی در جهت تماشای ادیتور روی کیبورد در ویندوز و مک کلمات زیر در کیبورد را همزمان بفشارید
```
Mac = Command + Shift + F
PC = Control + Shift + F
```

**Distance**

این برای پیدا کردن فاصله بین اجسام میباشد
```c#
float distance = Vector3.Distance(start position,end position);
```
