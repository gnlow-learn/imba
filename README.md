# imba

## memo

### imba bundler 사용 불가
```
Unable to create symlink for node_modules. If you're on Windows, try enabling "Developer Mode" in Windows settings or creating a Vite project instead.
```

### SVG Component 사용 불가?
- 이것 때문에 못 쓸듯..ㅜ
```
core.web.imba:560 Uncaught InvalidCharacterError: Failed to execute 'createElementNS' on 'Document': The qualified name provided ('class Block extends imba_Component {
	render(){
		var $1, $2, $3, $5 = this._ns_ || '', $6;
		$1=this;
		$1[$beforeReconcile$]();
		($2=$3=1,$1[$4] === 1) || ($2=$3=0,$1[$4]=1);
		$2 || ($6=imba_createSVGElement('g',$1,`${$5}`,null));
		;
		$1[$afterReconcile$]($3);
		return $1;
	}
	static {
		register$(this,c$0,'Block',2);
		imba_defineTag('block-o63xs0-ah',this,{name: 'Block'});
	}
}') contains the invalid character ' '.
    at createSVGElement (core.web.imba:560:31)
    at App.render (main.imba:25:13)
    at App.commit (component.imba:202:23)
    at App.visit (component.imba:192:15)
    at [#afterVisit] (component.imba:313:8)
    at main.imba:40:27
```