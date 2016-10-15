http://qiita.com/koba04/items/66e9c5be8f2e31f28461

|component|trigger|memo|
|:--|:--|:--|
|componentWillMount|コンポーネントのDOMツリー追加前|初期化|
|componentDidMount|コンポーネントのDOMツリー追加後|初期化/鯖レンダリングで不要な部分を記述|
|componentWillReceiveProps|Prop更新時|Propに応じてStateを変更する場合等|
|shouldComponentUpdate|コンポーネントのrerender前|falseを返すとrerenderされない, forceUpdateでは呼ばれない|
|componentWillUpdate|コンポーネントの更新前|setStateが使えない,componentWillReceivePropsを使え|
|componentDidUpdate|コンポーネントの更新後|DOMの変化に応じて何かするとき使える|
|componentWillUnmount|コンポーネントのDOMツリー削除時|ComponentDidMountで登録したTimerの処理やDOMの削除|