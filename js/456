
window.onload=function(){
		var oMore = document.getElementById('content-box');
		var ul = document.getElementById('ul-title');
		var oA = ul.getElementsByTagName('a');
		var arr = [0,-375,-1125];
		var setNum = 0;
		for(var i = 0;i<oA.length;i++){
			oA[i].num = i;
			oA[i].onclick=function(){
				setNum=0;
				var iNum = this.num;
				var oLeft = parseInt(oMore.style.left);
				var timer = setInterval(function(){
					if(arr[iNum]<oLeft){
						setNum = setNum-5;
						if(iNum == oLeft){
							clearInterval(timer);
							setNum = arr[iNum];
							oMore.style.left = setNum+'px';
						}else{
							if(setNum == arr[iNum]){
								clearInterval(timer);
								oMore.style.left = arr[iNum]+'px';	
							}else{
								oMore.style.left = setNum+'px';
							}
						}
					}else{
						setNum = setNum+5;
						if(iNum==oLeft){
							clearInterval(timer);
							setNum = arr[iNum];
							oMore.style.left = setNum+'px';

						}else{
							if(setNum == arr[iNum]){
								clearInterval(timer);
								oMore.style.left = arr[iNum]+'px';	
							}else{
								oMore.style.left = setNum+'px';
	
							}
						}						
					}
					
					

				},50);
				
			}
		}
	}