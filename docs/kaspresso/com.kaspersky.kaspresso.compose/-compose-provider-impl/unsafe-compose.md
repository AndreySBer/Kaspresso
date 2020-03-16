[kaspresso](../../index.md) / [com.kaspersky.kaspresso.compose](../index.md) / [ComposeProviderImpl](index.md) / [unsafeCompose](./unsafe-compose.md)

# unsafeCompose

`fun unsafeCompose(block: `[`ActionsOnElementsPack`](../../com.kaspersky.kaspresso.compose.pack/-actions-on-elements-pack/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Overrides [ComposeProvider.unsafeCompose](../-compose-provider/unsafe-compose.md)


`fun <Type> `[`Type`](unsafe-compose.md#Type)`.unsafeCompose(block: `[`ActionsPack`](../../com.kaspersky.kaspresso.compose.pack/-actions-pack/index.md)`<`[`Type`](unsafe-compose.md#Type)`>.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)` where Type : BaseActions, Type : BaseAssertions, Type : Interceptable<ViewInteraction, ViewAssertion, ViewAction>`
`fun <Type> `[`Type`](unsafe-compose.md#Type)`.unsafeCompose(block: `[`ActionsPack`](../../com.kaspersky.kaspresso.compose.pack/-actions-pack/index.md)`<`[`Type`](unsafe-compose.md#Type)`>.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)` where Type : UiBaseActions, Type : UiBaseAssertions, Type : UiInterceptable<UiObjectInteraction, UiObjectAssertion, UiObjectAction>`

Overrides [ComposeProvider.unsafeCompose](../-compose-provider/unsafe-compose.md)

Composes a [block](../-compose-provider/unsafe-compose.md#com.kaspersky.kaspresso.compose.ComposeProvider$unsafeCompose(kotlin.Function1((com.kaspersky.kaspresso.compose.pack.ActionsOnElementsPack, kotlin.Unit)))/block) of actions with their views to invoke on in one composite action that succeeds if at least
one of it's parts succeeds.
Please, be aware of `or` sections are executing without flakySafely mechanism
    even though there may be flakySafely interceptors in your Kaspresso settings!

### Parameters

`block` - the actions to compose.