let imgNum = document.querySelectorAll('td:nth-child(2)');
let imgValuesNum = [];
imgNum.forEach(function(singleCell) {
	imgValuesNum.push(singleCell.innerText);
}
);


let imgAlt = document.querySelectorAll('td:nth-child(4)');
let imgValuesAlt = [];
imgAlt.forEach(function(singleCell) {
	imgValuesAlt.push(singleCell.innerText);
}
);

let imgLink = [];

for (var i = 0; i < imgValuesAlt.length; i++) {

	console.log('<img style="width: 20%;" class="fr-fic fr-dii fr-fir" src="/ImageRepository/Document?documentId=' + imgValuesNum[i] + '" alt="' + imgValuesAlt[i] + '">');
}