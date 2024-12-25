เปลี่ยนเป็นคำทำนาย 3 ภาษา

css 

#paper {
            width: 400px;
            height: 732px;
            background-image: url('https://semicon.github.io/img/web/transparent_bg.png');
            background-size: cover;
            background-position: center;
            margin-bottom: 20px;
            display: none;
        }


ฟังก์ชั่นเปลี่ยนรูปภาพใบคำทำนาย

            function changeBackground() {
                const randomImage = Math.floor(Math.random() * 28) + 1;
                const formattedRandomImage = randomImage > 9 ? randomImage.toString() : `0${randomImage}`;

                console.log(randomImage);
                paper.style.backgroundImage = `url('https://www.liangchiang.com/gameImages/CM${formattedRandomImage}-1.jpg')`;
            }
