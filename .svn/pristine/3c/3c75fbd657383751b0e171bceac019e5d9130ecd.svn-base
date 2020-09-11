import { Injectable } from '@angular/core';
import { LoadingController } from 'ionic-angular';

@Injectable({
  providedIn: 'root'
})
export class LoadingService {

	isLoading = false;
	loader;
	
	constructor(public loadingController: LoadingController) { }

	async loadingFunction() {
		this.loader = await this.loadingController.create({
			spinner: 'crescent',
			content: 'Please wait while the data is initially set up for you...'
		})
		await this.loader.present();
	 }

	async loaderDismiss(){
	   await this.loader.dismiss();
	}

}