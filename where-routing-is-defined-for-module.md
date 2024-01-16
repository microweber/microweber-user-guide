# Where routing is defined for module?

Here is an example module on Livewire. \
https://github.com/microweber-modules/todo-module-livewire \
You can use the Laravel structure, but you need to load the service provider for the module in the config.php file and the namespace (to put your own).\
\
$config\['settings']\['autoload\_namespace'] = \[\
&#x20;\[ \
'path' => \_\_DIR\_\_ . '/src/', \
'namespace' => 'MicroweberPackages\\\Modules\\\TodoModuleLivewire\\\\' \
], \
]; \
You can find some example modules here [https://github.com/microweber-modules](https://github.com/microweber-modules)
