# custom-directive

Custom Directive adalah atribut kustom yang ada di Vue.js seperti halnya *v-if* dan <i>v-html</i>. Di Vue.js bisa dibuat kustom directive alias sesuai selera. Ada scope / jarak yaitu Global ( App.vue ) dan local ( di setiap component )

## Global Scope
<tt>
<pre>
  Vue.directive('namaDirective', {
    bind(el, binding, vnode){}
  });
</pre>
</tt>

## Local Scope
<tt>
<pre>
  directive:{
    namaDirective:{
      bind(el, binding, vnode){}
    }
  }
</pre>
</tt>

Pemanggilan dalam attribut HTML adalah *v-namaDirective*
