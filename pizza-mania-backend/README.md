

## 💳 Payment Integration

The application uses the **Stripe Android SDK** to handle credit card transactions securely.

* **Stripe Card Input Widget:** Provides a pre-built, secure UI for collecting card numbers, expiry dates, and CVC codes.
* **PCI Compliance:** Card data is sent directly to Stripe’s servers, ensuring sensitive information never touches the application backend.
* **Tokenization:** Converts card details into secure tokens for backend processing.

---
## 🚀 Setup & Installation

1. **Open Android Studio** and import the `CW1` folder.
2. **Stripe Configuration:**
* Obtain your **Publishable Key** from the [Stripe Dashboard](https://dashboard.stripe.com/).
* Initialize the SDK in your `Application` class or `PaymentActivity`:
```java
PaymentConfiguration.init(getApplicationContext(), "your_publishable_key_here");

```

## 🧪 Testing Payments

To test the payment flow, use Stripe's [test card numbers](https://www.google.com/search?q=https://stripe.com/docs/testing%23cards).

* **Test Card:** `4242 4242 4242 4242`
* **CVC:** Any 3 digits
* **Expiry:** Any future date

---
