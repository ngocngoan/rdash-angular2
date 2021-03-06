# Introduction

[AngularJS 2](https://angular.io/) implementation of the [RDash admin dashboard](http://rdash.github.io) theme

> Responsive, bloat free, bootstrap powered admin style dashboard!

[**Demo App**](https://rdash-angular2.herokuapp.com/)

# How to start

```bash
git clone https://github.com/ziyasal/rdash-angular2.git
cd rdash-angular2
npm install
# dev
npm start
```

## Components

- RdWidget
- RdWidgetHeader
- RdWidgetBody
- RdWidgetFooter
- RdLoading


**Simple Widget** 
```js
    <rd-widget>
      <rd-widget-body>       
       <span>HTML CONTENT</span>       
      </rd-widget-body>
    </rd-widget>
```

**Widget with Header**  
```js
 <rd-widget>
       <rd-widget-header icon="fa-tasks" title="Servers">
         <a href="javascript:void(0)" style="float: right">Manage</a>
       </rd-widget-header>
       <rd-widget-body classes="medium no-padding">
         <server-list-view [model]="servers"></server-list-view>
       </rd-widget-body>
     </rd-widget>
```

**Widget with Footer**  
```js
 <rd-widget>
       <rd-widget-header icon="fa-tasks" title="Servers">
         <a href="javascript:void(0)" style="float: right">Manage</a>
       </rd-widget-header>
       <rd-widget-body classes="medium no-padding">
         <server-list-view [model]="servers"></server-list-view>
       </rd-widget-body>
       <rd-widget-footer>
         <span>FOOTER CONTENT</span>
       </rd-widget-footer>
     </rd-widget>
```

**Widget with Loader**  
```js
 <rd-widget>
    <rd-widget-body classes="medium no-padding">
       <rd-loading></rd-loading>
    </rd-widget-body>
 </rd-widget>
```

# License

[MIT](https://raw.githubusercontent.com/ziyasal/rdash-angular2/master/LICENSE)
