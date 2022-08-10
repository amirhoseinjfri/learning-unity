**Clamp**
برای استفاده از (clamp) ابتدا باید مثلا از مکان یک جسم یک متغییر موقت بسازید مانند (temPos) سپس تغییرات را روی مقدار موقت انجام داده و سپس تغییرات انجام شده را روی مکان اصلی و فعلی انجام بدهید مانند مثال زیر

```c#
Vector3 tmpPos = transform.position;
tmpPos.x = Mathf.Clamp(tmpPos.x, -2.0f, 2.0f);
transform.position = tmpPos;
```
