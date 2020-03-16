[kaspresso](../../index.md) / [com.kaspersky.kaspresso.interceptors.behaviorkautomator.impl.flakysafety](../index.md) / [FlakySafeObjectBehaviorInterceptor](index.md) / [interceptPerform](./intercept-perform.md)

# interceptPerform

`fun <T> interceptPerform(interaction: UiObjectInteraction, action: UiObjectAction, activity: () -> `[`T`](intercept-perform.md#T)`): `[`T`](intercept-perform.md#T)

Overrides [KautomatorBehaviorInterceptor.interceptPerform](../../com.kaspersky.kaspresso.interceptors.behaviorkautomator/-kautomator-behavior-interceptor/intercept-perform.md)

Wraps the given [activity](intercept-perform.md#com.kaspersky.kaspresso.interceptors.behaviorkautomator.impl.flakysafety.FlakySafeObjectBehaviorInterceptor$interceptPerform(com.kaspersky.components.kautomator.intercept.interaction.UiObjectInteraction, com.kaspersky.components.kautomator.intercept.operation.UiOperation((androidx.test.uiautomator.UiObject2)), kotlin.Function0((com.kaspersky.kaspresso.interceptors.behaviorkautomator.impl.flakysafety.FlakySafeObjectBehaviorInterceptor.interceptPerform.T)))/activity) invocation with the flaky safety.

### Parameters

`interaction` - the intercepted [UiObjectInteraction](#).

`action` - the intercepted [UiObjectAction](#).

`activity` - the activity to invoke.