Angular 
ek framework hai jo large aur interactive web applications banane ke liye use hota hai.
....................................................................
           Component in angular 
   NavbarComponent
   BannerComponent
   ProductComponent
   AboutComponent
   FooterComponent.

import { Component } from '@angular/core';

@Component({
  selector: 'app-navbar',
  templateUrl: './navbar.component.html',
  styleUrl: './navbar.component.css'
})
export class NavbarComponent {

}
....................................................................
   Angular installation and project structure and cli 

Cli
Angular CLI = Angular project کو command line سے بنانے اور manage کرنے کا tool۔
....................................................................
*Ng for 
HTML میں بار بار دکھانے کے لیے ہوتا ہے۔
<h2>Students</h2>

<ul>
  <li *ngFor="let student of students">
    {{ student }}
  </li>
</ul>
....................................................................
      {{        }}
اس کا کام TypeScript کا data HTML میں display کرنا ہے۔
<h1>Hello {{ name }}</h1>
<p>Age: {{ age }}</p>
....................................................................
Custom Directives
 کیا ہے؟مثلاً ہم چاہتے ہیں کہ mouse لے جانے پر text کا background تبدیل ہو جائے۔
import { Directive, ElementRef } from '@angular/core';

@Directive({
  selector: '[appHighlight]'
})
export class HighlightDirective {

  constructor(private el: ElementRef) {
    this.el.nativeElement.style.backgroundColor = 'yellow';
  }

}
....................................................................
on click event emit Todo app
....................................................................
*Ng if 
         <p *ngIf="condition">
  Hello
</p>
اگر condition true ہو → <p> نظر آئے گا
اگر condition false ہو → <p> نظر نہیں آئے گا۔
....................................................................










                    
