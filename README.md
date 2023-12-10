# webpublish
Team CyIVA 만세!

2학년 기말 프로젝트로 진행되고 있는 웹 개발 프로젝트

개발환경은 QHD 21:9 환경으로, 화면 해상도에 따라 최대한 유연하게 반응하게 개발중입니다.
성적도 중요하지만, 과제 점수가 낮게 나오더라도 새로운것, 필요한것을 더 우선적으로 보고 있습니다.

js는 기본적인 코드를 스파게티로 짜고, 챗 지피티와 함께 예쁘게 정리하는 과정을 활용했습니다.

<script>
    document.addEventListener('DOMContentLoaded', function () { 
    var gearsHand1 = document.querySelector('.gears_hover.gears_hand1');
    var guideHand1 = document.querySelector('.guide.guidehand');
//구현 가능성 실험
    gearsHand1.addEventListener('mouseover', function () {
        if (guideHand1) {
            guideHand1.style.display = 'block';
        }
    });

    gearsHand1.addEventListener('mouseout', function () {
        if (guideHand1) {
            guideHand1.style.display = 'none';
        }
    });

   
    var gearsHand2 = document.querySelector('.gears_hover.gears_hand2');
    var guideHand2 = document.querySelector('.guide.guidehand');

    gearsHand2.addEventListener('mouseover', function () {
        if (guideHand2) {
            guideHand2.style.display = 'block';
        }
    });

    gearsHand2.addEventListener('mouseout', function () {
        if (guideHand2) {
            guideHand2.style.display = 'none';
        }
    });

//2개 동시 구현 가능성 실험
    var gearsArm1 = document.querySelector('.gears_hover.gears_arm1');
    var gearsArm2 = document.querySelector('.gears_hover.gears_arm2');
    var guideArm = document.querySelector('.guide.guidearm');

    gearsArm1.addEventListener('mouseover', function () {
        if (guideArm) {
            guideArm.style.display = 'block';
        }
    });

    gearsArm1.addEventListener('mouseout', function () {
        if (guideArm) {
            guideArm.style.display = 'none';
        }
    });

    gearsArm2.addEventListener('mouseover', function () {
        if (guideArm) {
            guideArm.style.display = 'block';
        }
    });

    gearsArm2.addEventListener('mouseout', function () {
        if (guideArm) {
            guideArm.style.display = 'none';
        }
    });

    var gearsleg1 = document.querySelector('.gears_hover.gears_leg1');
    var gearsleg2 = document.querySelector('.gears_hover.gears_leg2');
    var guideleg = document.querySelector('.guide.guideleg');

    gearsleg1.addEventListener('mouseover', function () {
        if (guideleg) {
            guideleg.style.display = 'block';
        }
    });

    gearsleg1.addEventListener('mouseout', function () {
        if (guideleg) {
            guideleg.style.display = 'none';
        }
    });

    gearsleg2.addEventListener('mouseover', function () {
        if (guideleg) {
            guideleg.style.display = 'block';
        }
    });

    gearsleg2.addEventListener('mouseout', function () {
        if (guideleg) {
            guideleg.style.display = 'none';
        }
    });

    var gearsShoes1 = document.querySelector('.gears_hover.gears_shoe1');
    var gearsShoes2 = document.querySelector('.gears_hover.gears_shoe2');
    var guideShoes = document.querySelector('.guide.guideshoes');

    gearsShoes1.addEventListener('mouseover', function () {
        if (guideShoes) {
            guideShoes.style.display = 'block';
        }
    });

    gearsShoes1.addEventListener('mouseout', function () {
        if (guideShoes) {
            guideShoes.style.display = 'none';
        }
    });

    gearsShoes2.addEventListener('mouseover', function () {
        if (guideShoes) {
            guideShoes.style.display = 'block';
        }
    });

    gearsShoes2.addEventListener('mouseout', function () {
        if (guideShoes) {
            guideShoes.style.display = 'none';
        }
    });

    var gearsShoulder1 = document.querySelector('.gears_hover.gears_shoulder1');
    var gearsShoulder2 = document.querySelector('.gears_hover.gears_shoulder2');
    var guideShoulders = document.querySelector('.guide.guideshoulder');

    gearsShoulder1.addEventListener('mouseover', function () {
        if (guideShoulders) {
            guideShoulders.style.display = 'block';
        }
    });

    gearsShoulder1.addEventListener('mouseout', function () {
        if (guideShoulders) {
            guideShoulders.style.display = 'none';
        }
    });

    gearsShoulder2.addEventListener('mouseover', function () {
        if (guideShoulders) {
            guideShoulders.style.display = 'block';
        }
    });

    gearsShoulder2.addEventListener('mouseout', function () {
        if (guideShoulders) {
            guideShoulders.style.display = 'none';
        }
    });

    var gearsTorso = document.querySelector('.gears_hover.gears_torso');
    var guideTorso = document.querySelector('.guide.guidetorso');

    gearsTorso.addEventListener('mouseover', function () {
        if (guideTorso) {
            guideTorso.style.display = 'block';
        }
    });

    gearsTorso.addEventListener('mouseout', function () {
        if (guideTorso) {
            guideTorso.style.display = 'none';
        }
    });

    var gearsHead = document.querySelector('.gears_hover.gears_head');
    var guideHead = document.querySelector('.guide.guidehead');

    gearsHead.addEventListener('mouseover', function () {
        if (guideHead) {
            guideHead.style.display = 'block';
        }
    });

    gearsHead.addEventListener('mouseout', function () {
        if (guideHead) {
            guideHead.style.display = 'none';
        }
    });

    var gearsTasset = document.querySelector('.gears_hover.gears_tasset');
    var guideTasset = document.querySelector('.guide.guidetasset');

    gearsTasset.addEventListener('mouseover', function () {
        if (guideTasset) {
            guideTasset.style.display = 'block';
        }
    });

    gearsTasset.addEventListener('mouseout', function () {
        if (guideTasset) {
            guideTasset.style.display = 'none';
        }
    });
});



</script>

정도 되는 코드를

<script>
    document.addEventListener('DOMContentLoaded', function () {
    // 이전에 hover된 객체를 저장하기 위한 변수
    var previousHoveredGuide = null;

    // 함수를 정의하여 재사용 가능하도록 함
    function handleHover(gearElement, guideElement) {
        gearElement.addEventListener('mouseover', function () {
            if (previousHoveredGuide) {
                // 이전에 hover된 객체가 있으면 display를 none으로 변경
                previousHoveredGuide.style.display = 'none';
            }

            if (guideElement) {
                guideElement.style.display = 'block';
                // 현재 hover된 객체를 저장
                previousHoveredGuide = guideElement;
            }
        });

        gearElement.addEventListener('mouseout', function () {
            // 아무 작업도 하지 않음
        });
    }

    // 재사용 가능한 함수를 호출하여 이벤트 핸들링
    handleHover(
        document.querySelector('.gears_hover.gears_hand1'),
        document.querySelector('.guide.guidehand')
    );

    handleHover(
        document.querySelector('.gears_hover.gears_hand2'),
        document.querySelector('.guide.guidehand')
    );

    handleHover(
        document.querySelector('.gears_hover.gears_arm1'),
        document.querySelector('.guide.guidearm')
    );

    handleHover(
        document.querySelector('.gears_hover.gears_arm2'),
        document.querySelector('.guide.guidearm')
    );

    handleHover(
        document.querySelector('.gears_hover.gears_shoulder2'),
        document.querySelector('.guide.guideshoulder')
    );
    handleHover(
        document.querySelector('.gears_hover.gears_shoulder1'),
        document.querySelector('.guide.guideshoulder')
    );

    handleHover(
        document.querySelector('.gears_hover.gears_leg2'),
        document.querySelector('.guide.guideleg')
    );
    handleHover(
        document.querySelector('.gears_hover.gears_leg1'),
        document.querySelector('.guide.guideleg')
    );

    handleHover(
        document.querySelector('.gears_hover.gears_shoe2'),
        document.querySelector('.guide.guideshoes')
    );
    handleHover(
        document.querySelector('.gears_hover.gears_shoe1'),
        document.querySelector('.guide.guideshoes')
    );
    handleHover(
        document.querySelector('.gears_hover.gears_head'),
        document.querySelector('.guide.guidehead')
    );
    handleHover(
        document.querySelector('.gears_hover.gears_tasset'),
        document.querySelector('.guide.guidetasset')
    );
    handleHover(
        document.querySelector('.gears_hover.gears_torso'),
        document.querySelector('.guide.guidetorso')
    );
});
</script>

까지 단순화, 압축해줬습니다. 그저... 대 빛 황 지피티...

에헤~
