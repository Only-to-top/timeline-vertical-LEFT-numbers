# timeline-vertical-LEFT

CSS :
```css
/* Вертикальный таймлайн ЛЕВЫЙ */
.timeline {
  padding: 40px 0;
}
.timeline-item {
  padding: 10px 0;
  position: relative;
  background-color: #f4f4f4;
}
.timeline-item::before {
  content: '●';
  position: absolute;
  width: 1px;
  height: 100%;
  border-left: 2px dotted #999;
  color: #999;
  font-size: 60px;
  line-height: 15px;
  text-indent: -18px;
  z-index: 2;
}
.timeline-item::after {
  content: '1';
  position: absolute;
  top: 16px;
  color: #fff;
  font-size: 16px;
  line-height: 96%;
  text-indent: 86px;
  z-index: 3;
}
.timeline-item:nth-child(2)::after{content: '2';}
.timeline-item:nth-child(3)::after{content: '3';}
.timeline-item:nth-child(4)::after{content: '4';}
.timeline-item:nth-child(5)::after{content: '5';}
.timeline-item p {
  line-height: 1.4;
  margin: -4px 0 0 0;
  font-size: 14px;
  padding: 10px 15px;
  margin-left: 30px;
  background-color: #fff;
  border-left: 2px solid #999
}
.timeline-item .timeline-item-title {
  left: 20px;
}
.timeline-item::before {
  left: -1px; 
}
.timeline-item:last-child::before{
  border: none;
}
.timeline-item:last-child::after{
  text-indent: 85px;
}
.timeline-item::after {
  left: -90px; 
}
/* / Вертикальный таймлайн ЛЕВЫЙ */
```

HTML :
```html
<div class="timeline">
  <div class="container">
    <div class="row">
      <div class="col-md-12">

        <div class="col-12 timeline-item">
          <p>Скорость доставки</p>
        </div>
        <div class="col-12 timeline-item">
          <p>Низкая стоимость и быстрое прохождение растаможки, за которую отвечает грузоперевозчик <br>
          - отсутствие ограничений по весу и стоимости товара (от 10 кг для коммерческих грузов, и от 1 кг на доставку образцов и мелких товаров)</p>
        </div>
        <div class="col-12 timeline-item">
          <p>Возможность миксовать различные виды товаров в одну отправку</p>
        </div>
        <div class="col-12 timeline-item">
          <p>Сертификаты соответствия и уточнение торговых марок не являются обязательными</p>
        </div>
        <div class="col-12 timeline-item">
          <p>Возможность консолидировать товары от разных поставщиков на складе грузоперевозчика (бесплатная услуга для наших клиентов)</p>
        </div>

      </div>
    </div>
  </div>
</div>
```
