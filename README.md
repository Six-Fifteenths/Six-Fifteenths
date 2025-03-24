

<style>
	/* 头像卡片 */
	.author-img {
        position: relative; /* 设置相对定位 */
    }
    
    .author-box {
        text-align: center;
        padding: 20px;
        height: auto;
        border-bottom: 2px solid #ddd;
        font-size: 1.5em;
        /* 分割线 */
    }

    .author-img img {
        border-radius: 50%; /* 显示为圆形 */
        width: 150px; /* 宽度设置 */
        height: 150px; /* 高度保持一致，否则就成椭圆了 */
        margin-bottom: 10px;
    }
    
    /* 文本格式，全局 */
    .content h2 {
        margin-top: 0;
        margin-bottom: 0;
    }
    
    /* 设置每一节宽度，高度，长度等等 */
    .content .column {
		margin-top: 4px;
        margin-bottom: 4px;
        width: 65%;
        margin-left: 20px;
    }
    
    /* 给第一格个人信息进行适配 */
    .content .info-columns {
        margin: 10px 0;
    }

	/* 第一格的个人信息，我使用了表格，为了显示更多信息的同时不空出大部分地方，你们自行选择 */
    .content .row {
        display: flex;
        justify-content: space-between;
    }
    
    /* 每一节通用格式 */
    .section {
        display: flex;
        padding: 10px 0px 10px 0px;
        align-items: center;
        justify-content: space-between;
        border-bottom: none;
        /*margin-top: 20px;*/
        /*margin: 20px 10px 0 10px;*/
        border-radius: 10px;
        /*background-color: white;*/
        height: auto;
        /*box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);*/
    }
    
    /* 夜间适配，改变背景和相关阴影部分 */
    [data-theme=dark] .section {
        background-color: #2c2c2c;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
    }
    
    /* 节内图片所在位置相关格式，这里是因为我开了fancybox，也就是点击预览大图的效果，使图片被一个a所包裹，如果你关了请自行将该内容添加到下面的img中，其他位置对应调整 */
    .section a {
		width: 45%;
		height: 100%;
		transition: transform 0.5s ease; /* 添加过渡效果 */

    }
	
	/* 通用文字部分基础设置 */
    .section .content {
        width: 100%;
        /*margin: 20px 20px;*/
        max-height: 100%;
        overflow: hidden; /* 超出部分不好看，我给隐藏了，看不见也比超出强，不过这个可以通过修改各种宽度高度进行个性适配 */
        text-overflow: ellipsis;
        transition: width 0.5s ease, margin-left 0.3s ease; /* 添加过渡效果 */
    }
    
    /* 窄屏适配 */
    @media (max-width: 870px) {/* 当页面宽度小于870像素时 */
        /* 不显示图片 */
		.section a {
			display: none;
		}
		
		/* 将位置留给文字 */
		.section .content {
			width: 100%;
		}
		/* 高度自己调整，因为窄屏视野没有那么大，部分节窄一点宽一点不影响，但是最小仍然是之前设置的值，这个需要你们自己改 */
		.section {
		    height: auto;
		    min-height: 250px;
		}
		
    }
</style>

<div class="author-box">
    <div class="author-img">
        <img class="no-lightbox" src="/image/avatar.jpg">
    </div>
    <div class="image-dot"></div>
    <p>循此苦旅，直抵群星</p>
</div>

<div class="section">
    <div class="content">
        <div class="info-columns">
            <h2>个人信息</h2>
            <ul>
                <div class="row">
                    <div class="column">
                        <li>姓名: [已编辑]</li>
                        <li>性别: 男</li>
                        <li>学校: 北京大学</li>
                        <li>人格: INTP-T</li>
                    </div>
                    <div class="column">
                        <li>昵称: SixFifteenths</li>
                        <li>职业: 学生</li>
                        <li>届次: 2026</li>
                        <li>政治面貌: 群众</li>
                    </div>
                    <div class="column">
                        <li>出生: 2007.10</li>
                        <li>位置: 北京</li>
                        <li>专业: 无</li>
                        <li>原神: 启动</li>
                    </div>
                </div>
            </ul>
        </div>
    </div>
</div>

## 兴趣爱好
- 打牌+肉鸽+音游，爱好大部分类型的卡牌/肉鸽/音游，其中许多超过100小时，对扑克牌和骰子有额外热爱。此外是解谜类游戏/Puzzlehunt/ARG爱好者，对相关知识有研究。围棋业余一段，魔方盲拧玩家，这两个均已荒废。
- 数学爱好者，前数学竞赛生，喜爱着数学竞赛，但是无时无刻不希望结束数学竞赛生涯。数学竞赛中是代数不等式爱好者。非初等数学中对Bourbaki的思想和著作很感兴趣并且正在阅读学习。曾经是OI生。对法语和拉丁语具有兴趣并且正在学习法语。对哲学极感兴趣。
- 术曲/音游曲/电音爱好者，歌单中这三类居多，具歌词的歌多为日语，其中25时翻唱居多，但不会日语。对文学作品不感兴趣，但科幻小说，科普类作品和克系作品除外。没看过任何一部动漫。喜爱“25时”每个角色，尤其是东云绘名。
- 小众爱好者，对有趣的追求十分旺盛。热衷于建立完不成的计划，无论时间范围。
- 职业三分钟热度选手。被浪费/毒害的不同爱好应数以百计。职业折腾选手，被前面这一条筛选下来的都经过了长时间的折腾，包括这个博客。很多事情做完准备工作便失去兴趣。

## 关于我自己
到目前为止，只是一个自以为的天之骄子，从小在父母的熏陶下以为自己可以名垂数学史，以为自己已经看到了数学的本质，以为天上天下唯我独尊，最终至少到目前为止还只是一个小人物，并且还在线性代数和分析学中苦苦挣扎。

但是他并没有失败，因为还没有到他死亡的时刻，不确定性的东西还在前方。这个傻小子仍然怀抱着成为巨人的心。毕竟一个从小到大一直是天之骄子的孩子怎么可能随随便便认输呢？

总之，这个博客只是一个“热爱数学的孩子”的故事，而他永远都是孩子，无论之后是泯灭人间还是独步天下。

## 我的一些目标
我的目标大多数都隐晦玄虚地写在了关于页上，这些目标中既包含我的宏图伟业又包含我的兴趣爱好，这些留给各位作猜测。但是您们可以完全确定的是，我的最终目标永远是“为人类创造尽可能大的贡献”。

<div class="section">
    <div class="content">
        <h2>我的一些低概率事件</h2>
        <ul>
            <div class="row">
                    <div class="column">
                        <li>北京大学学生: 在全体同龄人中占比0.02%。</li>
                        <li>INTP: 占人类总数的3.3%。</li>
                        <li>双A共患确诊: 在全体成人中占约1%。</li>
                        <li>???: 在全体承认中占比1%。</li>
                        <li>幻????统???: 在全体??中占比??%。</li>
                    </div>
                    <div class="column">

                        <li>Phigros制霸: 在全体Phigros玩家中占比1%。</li>
                        <li>杀戮尖塔全成就: 在全体杀戮尖塔玩家中占比2.5%。</li>
                    </div>
            </div>
            <li>以上事件并不一定互相独立，但是仍然可以初步估计同时满足以上条件的在地球人中只有我一个。</li>
        </ul>
    </div>
</div>

{% hideToggle 我积累了一些中二病语句，您确定您想看吗？ %}


<div class="section">
    <div class="content">
        <h2>若干句中二式自我评价</h2>
        <ul>
            <div class="row">
                <div class="column">            
                    <li>如果退路让人怠惰，那就斩断退路逼迫一往无前。</li>
                    <li>怀揣匹夫之勇的傲慢之人，真的知道将要面对的是什么吗？</li>
                    <li>伴有痛苦的这份情感，可以称之为梦想吗？</li>
                    <li>如果矢志与所有的不合理斗争，结局就会是幸福的吗？</li>
                    <li>自卑过度？还是慕强过度？不卑不亢？还是逃避困难？</li>
                    <li>当终于面见了真正残酷的现实，还能保持所谓本心吗？</li>
                    <li>更快！更快！更快！走到他们之前，证明他们是错的！</li>
                    <li>迷茫中的人：若终于明白了自己的目标就去做吧。</li>
                    <li>科学无不可知：而我们必须知道，我们必将知道。</li>
                </div>
                <div class="column">
                    <li>所做的一切都只是为了回答一个问题：为什么？</li>
                    <li>只是为了证明我的选择是正确的：便至于让我做到这一步。</li>
                    <li>伊甸园中的孩子啊——如今你身处何方？往何处去？</li>
                    <li>我必须坚信，我所热爱和执着的事具有改变世界的力量。</li>
                    <li>能做事的做事，能发声的发声。有一分热，发一分光。</li>
                    <li>活下去，看下去，走下去——至少要看到那个未来。</li>
                    <li>选择孤独，并一直孤独下去，成为唯一的面壁者。</li>
                    <li>请不要嘲笑我，哪怕是卑微可笑的，梦。</li>
                    <li>故作坚强地不再哭泣有许久——你心中还剩什么呢？</li>
                </div>
            </div>
            <li>注: 以上若干条可能不止一条为真或为假。请根据您对我的了解自行甄别。</li>
        </ul>
    </div>
</div>


{% endhideToggle %}


<div class="section">
    <div class="content">
        <h2>其他Q&A</h2>
            <div class="row">
                    <div class="column">
                        <li>Q: 为什么起昵称为十五分之六这个怪名字？</li>
                        <li>A: 有一次我在关键考试中没约分导致痛失入选后痛定思痛起的名字。后来发现这个名字十分好看并且符合命名规律就留下来了。我在互联网上的身份不算太少，这个最多。有唯一特征可以确认互联网上某个身份是不是我————是什么呢？（笑）</li>
                        <li>Q: 小百合，有没有什么不能忘记的人？</li>
                        <li>A: 有两个李姓朋友我不会忘记。一位是李克正，一位是李归农。我立志走数学道路一定程度上有他们二位“功劳”。李归农是因为种族歧视让我绷不住了，李克正则是有一次数学竞赛中明晃晃的当场修改规则让我愤怒，事实上我会记下学习路上的每一个阻碍，包括那些毫不顾忌嘲笑和阻碍中国数学的人————然后超过去。</li>
                        <li>Q: 你和527什么关系？</li>
                        <li>A: 真的只是朋友而已（心虚）只是从高中起就认识的一个同年同月同日生的朋友罢了，你无需知道更多。</li>
                    </div>
                    <div class="column">
                        <li>Q: 你是怎么走上数学这条不归路的？</li>
                        <li>A: 一开始是被朋友忽悠着报了学而思，结果入学测就搞了个满分被忽悠进第二高班型，自此命运的齿轮开始转动（笑）之后就到了最高班型里呆着，发现之上的数学竞赛与高等的数学可以帮助我看到真正漂亮的数学结果，还能送我进北大，就毫不犹豫地往前冲了。事实上原因只有一个，就是我想看真正漂亮的数学。</li>
                        <li>Q: 如何看待中国IMO冠军金牌频出却无一菲尔兹奖，最好大学在世界排不上号？</li>
                        <li>A: 很简单，我成尊不就是了？</li>
                        <li>Q: 现在想做什么，以后想做什么？</li>
                        <li>A: 现在的话想把博客和笔记的运行循环完完整整弄好，把我要精简的东西精简完，然后把数学基础打得扎实一点。以后的话想尽量成尊（笑）不成尊也没关系，能出一份力算一份。</li>
                    </div>
                </div>
    </div>
</div>


## 联系方式
- QQ: 3399155160
- domain mail: admin@infplus.me
- X: shtneetfiFxiS
- 以上这些平台是我所有能告诉您的。
