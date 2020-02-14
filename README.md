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

## Argumen Pada Bind()
### Argumen Pertama
Digunakan untuk mengembalikan nilai berupa element HTML

### Argumen Kedua
Digunakan untuk memproses data yang berhubungan dengan Custom Directive

## Value, Arg, dan Modifiers
### Value
Adalah nilai yang diambil dari nilai atribut custom directive tersebut , misalkan
<pre>
<tt>
v-namaDirective="'red'"
</tt>
</pre>
*'red'* adalah value

### Arg
<pre>
<tt>
v-namaDirective:myArg="'red'"
</tt>
</pre>
*myArg* adalah argument atau arg

### Modifiers
<pre>
<tt>
v-namaDirective.mod="'red'"
</tt>
</pre>
*mod* adalah modifiers
