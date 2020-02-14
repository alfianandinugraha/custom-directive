# custom-directive

Custom Directive adalah atribut kustom yang ada di Vue.js seperti halnya *v-if* dan <i>v-html</i>. Di Vue.js bisa dibuat kustom directive alias sesuai selera. Ada scope / jarak yaitu Global ( App.vue ) dan local ( di setiap component )

## Global Scope
<pre>
<tt>
  Vue.directive('namaDirective', {
    bind(el, binding, vnode){}
  });
</tt>
</pre>

## Local Scope
<pre>
<tt>
  directive:{
    namaDirective:{
      bind(el, binding, vnode){}
    }
  }
</tt>
</pre>

Pemanggilan dalam attribut HTML adalah *v-namaDirective*
