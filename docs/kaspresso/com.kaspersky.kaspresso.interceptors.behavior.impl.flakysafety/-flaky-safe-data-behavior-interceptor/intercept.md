[kaspresso](../../index.md) / [com.kaspersky.kaspresso.interceptors.behavior.impl.flakysafety](../index.md) / [FlakySafeDataBehaviorInterceptor](index.md) / [intercept](./intercept.md)

# intercept

`fun <T> intercept(interaction: DataInteraction, action: () -> `[`T`](intercept.md#T)`): `[`T`](intercept.md#T)

Overrides [BehaviorInterceptor.intercept](../../com.kaspersky.kaspresso.interceptors.behavior/-behavior-interceptor/intercept.md)

Wraps the given [action](intercept.md#com.kaspersky.kaspresso.interceptors.behavior.impl.flakysafety.FlakySafeDataBehaviorInterceptor$intercept(androidx.test.espresso.DataInteraction, kotlin.Function0((com.kaspersky.kaspresso.interceptors.behavior.impl.flakysafety.FlakySafeDataBehaviorInterceptor.intercept.T)))/action) invocation with the flaky safety.

### Parameters

`interaction` - the intercepted [DataInteraction](#).

`action` - the action to invoke.