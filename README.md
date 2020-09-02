Học css
--- Có thể xem các thuộc tính trên gg gõ css cheat sheet.
1. Font trong css.
	- font-family: Kiểu chữ trong css.
	- font-weight: normal/bold.
2. Spacing trong css: padding, margin.
	- padding: Là khoảng cách. giữa đường viền với nội dung bên trong( Có màu xanh lá trong chrome developer tools). Cú pháp:
		+ padding-top: Khoảng-cách..
		+ padding-right: Khoảng-cách..
		+ padding-bottom: Khoảng-cách..
		+ padding-left: Khoảng-cách..
		+ padding: top right bottom left.
		+ padding: top right-left bottom.
		+ padding: top-bottom right-left.
		+ padding: Tất-cả.
	-margin: Là khoảng cách. giữa các div với nhau( Có màu vàng cam trong chrome developer tools). Cú pháp:
		+ margin-top: Khoảng-cách..
		+ margin-right: Khoảng-cách..
		+ margin-bottom: Khoảng-cách..
		+ margin-left: Khoảng-cách..
		+ margin: top right bottom left.
		+ margin: top right-left bottom.
		+ margin: top-bottom right-left.
		+ margin: Tất-cả.
3. Border.
	- border-style: solid | dotted | dashed...
	- border-width: Khoảng-cách.
	- border-color: Màu.
	- Shorthand:
		+ border: solid 10px red.
	- border-top-width.
	- border-right-width.
	- border-width: top right bottom left.
4. Background-color: Bao gồm cả padding lẫn content.
	- background-color: Màu.
	- background-color: transparent( Màu trong suốt, có thể thấy được nền của layer đã bị chồng).
	- background-color: Gradient( Kiểu thay đổi nhiều màu, lên gg gõ background gradient generator).
5. Background-image: Ảnh nền.
	- background-image: url('Đường-dẫn') | none.
	- background-size: %( Kích cỡ của ảnh).
	- background-attachment: fixed | scroll*.
	- background-clip: border-box* | padding-box | content-box( Chế độ bao phủ: từ border, padding, content).
	- background-position.
	- background-repeat: repeat* | no-repeat | repeat-x | repeat-y | space | round.
	- background-size: auto | contain | cover.
6. Icons: https://fontawesome.com
7. Styling link: Có thể dùng với nhiều thẻ khác nhưng chỉ nên dùng với thẻ a.
	- a:link: Dùng để hiển thị đường dẫn ban đầu.
	- a:visited: Dùng để hiển thị khi đã nhấn vào đường dẫn.
	- a:hover: Dùng để hiển thị đặt trỏ chuột lên đường dẫn( Phải đứng sau link và active mới có hiệu quả).
	- a:active: Dùng để hiển thị khi nhấn giữ không buông chuột( Phải đứng sau  hover mới có hiệu quả).
8. Table.
	- Gồm các thẻ: table, tr, th, td.
	- border-collapse: seperated* | collapse.
	- vertical-align: top | middle | bottom.
	- text-align: left | center | right.
	- th, td không có margin.
	- Có thể dùng hover cho table, tr, td, th.
	- Tô màu nền theo quy luật: :nth-child(an+b) hoặc :nth-child(even | odd).
9. Lists: ul, li, ol.
	- list-style-type: none | square | circle | upper/lower roman/alpha.
	- list-style-position: inside | outside.
	- list-style-image: url('filepath').
	- list-style: type position image.
10. Display: inline vs block.
	- inline: Chiều rộng bằng nội dung của nó, có thể nằm cùng 1 hàng với các inline element khác.
	- block: Chiếm trọn 1 hàng.
	- Có thể chuyển từ trạng thái inline sang block và ngược lại bằng cách thêm css 
		{
			display: inline/block
		}

	|  | inline | block |
	| --- | --- | --- |
	| width, height | Không thay đổi | Có thay đổi |
	| --- | --- | --- |
	| margin | Thay đổi left, right | Thay đổi tất cả |
	| | Không thay đổi top, bottom |  |
	| --- | --- | --- |
	| padding | Có thể thay đổi cả 4 | Có thể thay đổi cả 4 |
11. CSS Combinators. Có 4 kiểu:

	- Desendant selector( Dùng dấu cách).

	VD: .list1 li nghĩa là tất cả những thẻ li nằm trong class list1 sẽ được chọn( Nghĩa là những thẻ li là con, cháu,... của class list1).

	- Child selector( Dùng dấu >).

	VD: .list1 > li nghĩa là chỉ những thẻ li là thẻ con nằm trong class list1 mới được chọn, không chọn thẻ li là cháu, chút, chít... của class list1.

	- Adjacent sibling selector( Dùng dấu +): Phải cùng hàng, cùng thẻ cha vì nó là anh chị em, và chỉ chọn 1 cái kế tiếp ngay sau giống với bộ kết hợp.

	VD: .list1 + ul nghĩa là chọn thẻ ul ngang hàng với class list1 và ngay sau là ul class list2 và chỉ chọn 1 ul class list2 không chọn tiếp ul class list3.

	- General sibling selector( Dùng dấu ~): Phải ngang hàng, cùng thẻ cha vì nó là anh chị em, chọn tất những anh chị em sau nó đúng với bộ chọn.
	VD: .list1 ~ ul nghĩa là chọn tất cả những thẻ ul ngang hàng, đứng sau nó, đó là ul.list2 và cả ul.list3.
12. Flexbox: Có 1 số thuộc tính là của cha và một số thuộc tính của con.
	- Thuộc tính thuộc về cha( .flex-container):
		+ display: flex;
		+ flex-direction: row* | column | row-reverse | column-reverse.
		+ flex-wrap: nowrap* | wrap | wrap-reverse.
		+ justify-content: Là căn chỉnh có hướng cùng hướng với flex-direction( row - ngang, column - dọc).
			flex-start* | flex-end | center | space-between | space-around | space-evenly
			flex-start: Mặc định.
			flex-end: Căn giá trị nằm cuối của thẻ cha.
			center: Căn giữa.
			space-between: Căn cho khoảng cách giữa các .item bằng nhau, nhưng không có khoảng cách đầu và cuối.
			space-around: Căn cho khoảng cách các .item gấp đôi khoảng cách đầu và cuối.
			space-evenly: Căn cho khoảng cách đầu, cuối, giữa các .item bằng nhau.
		+ align-items: Là căn chỉnh có hướng vuông góc với hướng của flex-direction.
			flex-start | flex-end | center | stretch* | baseline
			flex-start: Là cho nằm đầu .container.
			flex-end: Căn nằm cuối .container.
			center: Nằm giữa .container.
			stretch: Mặc định, kéo dài cho bằng với độ dài .container.
			baseline: Chỉnh cho nội dung nằm trên 1 trục theo chiều flex-direction.
		+ align-content: Căn chỉnh nội dung giữa các dòng.
			flex-start | flex-end | center | stretch* | space-between | space-round | space-evenly.
	- Thuộc tính thuộc về con( .item):
		+ flex-basis: Chỉnh độ dài ban đầu cho mỗi .item con nằm trong .flex-container là flexbox, dãn theo chiều của flex-direction.
		+ flex-grow: Chia khoảng không gian trống của flexbox cha để thêm vào flex con theo tỉ lệ của flex-grow flex con nảy trên tổng số flex-grow của các flex con.
			flex-grow: 0* | Number( Không âm).
		+ flex-shrink: Chia khoảng không gian thiếu của flexbox ra cho các flex con.
			flex-shrink: 1* | Number( Không âm, 0 thì flex con đó sẽ không bị co lại mà các flex con còn lại bị co).
			Công thức: flexBasis * ( 1 + flexShrinkNumber / Sum(shrink * flexBasis) * Phần-không-gian-bị-thiếu).
		+ order: Thay đổi thứ tự hiển thị của các flex con, số nhỏ trước lớn sau, theo thứ tự tăng dần.
			order: 0* | Number( Có thể là số âm).
		+ flex: <flex-grow> <flex-shrink> <flex-basis>
			Là cách viết tắt cho nhanh
		+ flex-self: Căn chỉnh cho flex con giống như các thuộc tính của align-items.
13. position: static* | relative | fixed | absolute | sticky.
	- Để thay đổi cần thêm thuộc tính cho đối tượng đó:
		top | right | bottom | left

	- relative: Thay đổi vị trí 1 cách tương đối so với vị trí ban đầu của nó mà không làm thay đổi bất kỳ vị trí của element nào xung quanh nó.

	- fixed: Thay đổi vị trí 1 cách tương đối so với màn hình cửa sổ trình duyệt, làm thay đổi ví trí của các thẻ xung quanh nó.

	- absolute: Thay đổi vị trí 1 cách tương đối so với thẻ bao, chứa nó có position: absolute gần nhất( Nghĩa là nó là con, cháu, chút, chít,... chứ không phải ngang hàng hoặc thấp hơn), và làm thay đổi vị trí của các thẻ có liên quan đến nó( Khá giống với position: fixed).

	- sticky: Thay đổi vị trí 1 cách tương đối so với màn hình giao diện của trình duyệt khi kéo thanh cuộn( Gần giống position: fixed nhưng đây là khi kéo thanh cuộn), sau đó kéo trở lại thì nó sẽ trở về vị trí cũ, không làm thay đổi vị trí của các element liên quan( Khác với position: fixed).

	***Chú ý: 
	 - Để căn giữa trung tâm thì cần thêm transform: translate(-50%, -50%).
	 - z-index: number;
	 	Chỉ thứ tự hiển thị khi chồng lên nhau.
	 	Chỉ sử dụng cho thuộc tính position.
	 	number là số nguyên( Có thể âm hoặc dương), number càng lớn thì xếp càng cao( Giống ngăn xếp càng cao càng nằm ngoài cùng , càng gần hiển thị).
	***
14. float: left | right.
	clear: left | right | both.
	Học được cách clearfix bằng cách sử dụng pseudo element after.
15. Transforms:
	- transform: translate(x-axis, y-axis)
		Dùng để di chuyển element từ ví trí hiện tại theo trục x và y.
		+ x dương hướng qua phải, x âm hướng qua trái.
		+ y dương hướng xuống dưới, âm hướng lên trên.
	- transform: rotate(<number>deg)
		Dùng để xoay element theo chiều kim đồng hồ hoặc ngược chiều kim đồng hồ.
		+ number > 0: Quay element theo chiều kim đồng hồ.
		+ number < 0: Quay element ngược chiều kim đồng hồ.
	- transform: scale(x-scale, y-scale)
		Dùng để phóng to, thu nhỏ kích thước ảnh ban đầu.
		+ x-scale: Thu phóng theo chiều ngang. Có 4 trường hợp:
			* x-scale > 1: Phóng to lên gấp x lần.
			* 0 < x-scale < 1: Thu nhỏ x lần.
			* -1 < x-scale < 0: Thu nhỏ |x| lần và đảo ngược element(Xoay 180 độ theo trục x).
			* x-scale < -1: Phóng to |x| lần và đảo ngược element( Xoay 180 độ theo trục x).
		+ y-scale: Thu phóng theo chiều dọc. Có 4 trường hợp:
			* y-scale > 1: Phóng to y lần.
			* 0 < y-scale < 1: Thu nhỏ y lần.
			* -1 < y-scale < 0: Thu nhỏ |y| lần và đảo ngược element( Xoay 180 độ theo trục y).
			* y-scale < -1: Phóng to |y| lần và đảo ngược element(Xoay 180 độ theo trục y).
		Có thể phóng to hay thu nhỏ 1 trục x hoặc y:
			+ scaleX(x-scale): Chỉ theo trục x.
			+ scaleY(y-scale): Chỉ theo trục y.
	- transform: skew(<x-skew>deg, <y-skew>deg)
		Dùng để xoay element theo cả trục x và trục y.
		+ x-skew: Dùng để xoay element theo trục x với x-skew độ.
		+ y-skew: Dùng để xoay element theo trục y với y-skew độ.
		Có thể dùng skew để xoay theo 1 trục x hoặc y.
		+ skewX(<x-skew>deg): Dùng để xoay element theo trục x.
		+ skewY(<y-skew>deg): Dùng để xoay element theo trục y.
		+ skew(<x-skew>deg): Dùng để xoay element theo trục x khi chỉ có 1 đối số.
	- transform: matrix(scaleX, skewX, skewY, scaleY, translateX, translateY).
16. Transitions: Dùng để điều chỉnh hiệu ứng khi thay đổi các thuộc tính của element khi được trỏ chuột vào.
	- transition: <transition-property> <transition-duration> <transition-timing-function> <transition-delay>
		+ transition-property: Dùng để chỉ định thuộc tính element bị transition ảnh hưởng khi thay đổi giá trị.
			transition-property: width[, height, .....]
		+ transition-duration: Dùng để chỉ định thời gian giới hạn khi dùng transition cho thuộc tính.
			transition-duration: time( Thường được tính bằng giây s hoặc mili giây ms).
		+ transition-timing-function: Dùng để thay đổi tốc độ khi dùng transition mỗi lúc nhanh chậm khác nhau(Xem thêm tại easings.net).
			transition-timing-function: ease* || linear || ease-in || ease-out || ease-in-out.
		+ transition-delay: Dùng để điều chỉnh độ trễ trước khi bắt đầu các hiệu ứng transition ảnh hưởng.
			transition-delay: time( Thường được dùng bằng giây s hoặc mili giây ms).
	- Có thể kết hợp với transforms:
		transition: transform <time(s)>;
			+ transform <time(s)>: Dùng để xác định thời gian giới hạn cho sự thay đổi của transform, thường được tính bằng giây. 