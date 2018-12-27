# angular

show-hide-password


Email: krolandaziawor@gmail.com | freelance web developer (symfony,java spring,angular)


================================ Angular 6 ====================================

Ce petit recaptulatif est fait en Angular 6 pour vous. L'objectif en fait est de créer une vue de login avec le visionnaire de password. Vous y êtes ?

                                                  OK allons y!!!!
                                                  
 Supposons que nous savons tous installer un projet angular sinon https://angular.io/guide/quickstart.
 
 Une fois le projet installé,
  
      1. vous aurez à integrer boostrap 4
      
          $ npm install  bootstrap --save
      
      2. installer ngx-show-hide-password
      
          $ npm install ngx-show-hide-password --save
          OH YES! Il ne suffit pas d'installer notre machin seulement. Il faut qu'on l'importe dans notre module de base.
                
         // app.module.ts      
        import { BrowserModule } from '@angular/platform-browser';
        import { NgModule } from '@angular/core';
        import { ShowHidePasswordModule } from 'ngx-show-hide-password';
        import { AppComponent } from './app.component';
        import { ClarityModule } from '@clr/angular';
        import { BrowserAnimationsModule } from '@angular/platform-browser/animations';
        import { AngularFontAwesomeModule } from 'angular-font-awesome';

          @NgModule({
            declarations: [
              AppComponent
            ],
            imports: [
              BrowserModule,
              ClarityModule,
              BrowserAnimationsModule,
              ShowHidePasswordModule.forRoot(),//importation du module ShowHidePassword
              AngularFontAwesomeModule  //Importation du module FontAwesomeModule
            ],
            providers: [],
            bootstrap: [AppComponent]
          })
      export class AppModule { }
                         
      3. installer angular font awesome
          $ npm install --save font-awesome angular-font-awesome
        
        Ajoutons ensuite le font-awesome.css dans notre fichier angular.json
        
           "styles": [
              "node_modules/bootstrap/dist/css/bootstrap.min.css",
              "src/styles.css",
              "node_modules/font-awesome/css/font-awesome.css"
            ],
          
 
 Une fois les integrations faites nous sommes donc en mesure d'avoir le resultat souhaité.
 
 Remarque: Le contenu du code est lisible et facile donc bonne chance à nous. On est ensemble!!!!!!!!!

References:
  - https://www.npmjs.com/package/ngx-show-hide-password
  - https://www.npmjs.com/package/angular-font-awesome
