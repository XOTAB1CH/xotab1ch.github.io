var table = document.getElementsByClassName("t")[0];

var questions = parseInt( table.getElementsByTagName("tr")[1].getElementsByTagName("td")[1].innerText.split('/')[0] ); //Задано (питань/балів)
for(let i = 1; i <= questions; i++){

	if(100 / questions * i >= 75.0)
	{
		table.getElementsByTagName("tr")[0].getElementsByTagName("td")[1].innerText = getRandomInt(3, 20).toString();//Спроб: 0
        table.getElementsByTagName("tr")[2].getElementsByTagName("td")[1].innerText = i.toString() + "/" + i.toString(); //Правильних відповідей
        table.getElementsByTagName("tr")[3].getElementsByTagName("td")[1].innerText = Math.floor(100 / questions * i).toString() + "%"; //Процент правильних балів
        document.getElementsByClassName("g")[1].innerText = Math.floor(100 / questions * i).toString() + "%";//Процент правильних балів
        document.getElementsByClassName("g")[2].innerText = table.getElementsByTagName("tr")[0].getElementsByTagName("td")[1].innerText;//Спроб
        document.getElementsByClassName("mark")[0].getElementsByTagName("img")[0].src = "https://xotab.cf/image/4.png";//Картинка оценка
        break;
	}
}

function getRandomInt(min, max) {
  min = Math.ceil(min);
  max = Math.floor(max);
  return Math.floor(Math.random() * (max - min)) + min; //Максимум не включается, минимум включается
}