```ts
class Seq.Keyed<K, V> extends Seq<K, V>, Collection.Keyed<K, V>
```

```ts
Seq.Keyed<K, V>(collection: Iterable<[K, V]>): Seq.Keyed<K, V>
Seq.Keyed<V>(obj: {[key: string]: V}): Seq.Keyed<string, V>
Seq.Keyed<K, V>(): Seq.Keyed<K, V>
Seq.Keyed(): Seq.Keyed<any, any>
```

---

- [toJS](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/toJS)
- [toJSON](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/toJSON)
- [toArray](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/toArray)

```ts
toJS(): Object
toJSON(): {[key: string]: V}
toArray(): Array<[K, V]>
```

- [toSeq](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/toSeq)

```ts
toSeq(): this
```

---

- [concat](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/concat)

```ts
concat<KC, VC>(...collections: Array<Iterable<[KC, VC]>>): Seq.Keyed<K | KC, V | VC>
concat<C>(...collections: Array<{[key: string]: C}>): Seq.Keyed<K | string, V | C>
```

---

- [map](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/map)

```ts
map<M>(
    mapper: (value: V, key: K, iter: this) => M,
    context?: any
): Seq.Keyed<K, M>
```

- [flatMap](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/flatMap)

```ts
flatMap<KM, VM>(
    mapper: (value: V, key: K, iter: this) => Iterable<[KM, VM]>,
    context?: any
): Seq.Keyed<KM, VM>
```

- [filter](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/filter)

```ts
filter<F>(
    predicate: (value: V, key: K, iter: this) => boolean,
    context?: any
): Seq.Keyed<K, F>

filter(
    predicate: (value: V, key: K, iter: this) => any,
    context?: any
): this
```

---

- [mapKeys](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/mapKeys)

```ts
mapKeys<M>(
    mapper: (key: K, value: V, iter: this) => M,
    context?: any
): Seq.Keyed<M, V>
```

- [mapEntries](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/mapEntries)

```ts
mapEntries<KM, VM>(
    mapper: (entry: [K, V], index: number, iter: this) => [KM, VM],
    context?: any
): Seq.Keyed<KM, VM>
```

- [flip](https://facebook.github.io/immutable-js/docs/#/Seq.Keyed/flip)

```ts
flip(): Seq.Keyed<V, K>
```
