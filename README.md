# Dart enum Extension

Easy Dart Enum

Made by Benjamin Mahmić ("https://github.com/BenjaminMahmic")

## How to use

1. Select complete enum

![Screenshot_1](https://github.com/BenjaminMahmic/dart_enum_extension/assets/89051381/24f90e41-03da-4815-9ec2-079bf7d2eefe)


2. Call Quick Fix (Windows: `Ctrl + .` or Mac: `⌘ + .`) and select `Generate (is)Enum Extension`

![Screenshot_2](https://github.com/BenjaminMahmic/dart_enum_extension/assets/89051381/b553cf95-0d87-4474-8d5e-8b539fbe082e)


3. That's it! 🎉

![Screenshot_3](https://github.com/BenjaminMahmic/dart_enum_extension/assets/89051381/77ed7716-1f38-4c4b-8583-3ded69b25e82)

## Example

```dart
  enum SubscriptionType {
    free,
    monthly,
    annal,
  }

  extension SubscriptionTypeExtension on SubscriptionType {
    bool get isFree => this == SubscriptionType.free;
    bool get isMonthly => this == SubscriptionType.monthly;
    bool get isAnnual => this == SubscriptionType.annual;
  }

  final subscriptionType = SubscriptionType.monthly;

  void main() {
    print(subscriptionType.isMonthly); // true
    print(subscriptionType.isAnnual); // false
  }
```

**Enjoy!** 🚀
