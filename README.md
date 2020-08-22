Học css
--- Có thể xem các thuộc tính trên gg gõ css cheat sheet.
1. Font trong css.
	- font-family: Kiểu chữ trong css.
	- font-weight: normal/bold.
2. Spacing trong css: padding, margin.
	- padding: Là khoảng cách. giữa đường viền với nội dung bên trong.( Có màu xanh lá trong chrome developer tools). Cú pháp:
		+ padding-top: Khoảng-cách..
		+ padding-right: Khoảng-cách..
		+ padding-bottom: Khoảng-cách..
		+ padding-left: Khoảng-cách..
		+ padding: top right bottom left.
		+ padding: top right-left bottom.
		+ padding: top-bottom right-left.
		+ padding: Tất-cả.
	-margin: Là khoảng cách. giữa các div với nhau.( Có màu vàng cam trong chrome developer tools). Cú pháp:
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
4. Background-color: bao gồm cả padding lẫn content.
	- background-color: Màu.
	- background-color: transparent.( Màu trong suốt, có thể thấy được nền của layer đã bị chồng)
	- background-color: Gradient.( Kiểu thay đổi nhiều màu, lên gg gõ background gradient generator)
5. Background-image: Ảnh nền.
	- background-image: url('Đường-dẫn') | none.
	- background-size: %.( Kích cỡ của ảnh)
	- background-attachment: fixed | scroll*.
	- background-clip: border-box* | padding-box | content-box.( Chế độ bao phủ: từ border, padding, content)
	- background-position.
	- background-repeat: repeat* | no-repeat | repeat-x | repeat-y | space | round.
	- background-size auto | contain | cover.
6. Icons: https://fontawesome.com
7. Styling link: Có thể dùng với nhiều thẻ khác nhưng chỉ nên dùng với thẻ a.
	- a:link: Dùng để hiển thị đường dẫn ban đầu.
	- a:hover: Dùng để hiển thị đặt trỏ chuột lên đường dẫn.
	- a:active: Dùng để hiển thị khi nhấn giữ không buông chuột.
	- a:visited: Dùng để hiển thị khi đã nhấn vào đường dẫn.
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
	- block: chiếm trọn 1 hàng.
	- Có thể chuyển từ trạng thái inline sang block và ngược lại bằng cách thêm css 
		{
			display: inline/block
		}

	|  | inline | block |
	| --- | --- | --- |
	| width, height |			Không thay đổi		  |      	Có thay đổi	            |
	| --- | --- | --- |
	|    margin     |      Thay đổi left, right       |        Thay đổi tất cả          |
	|				|      Không thay đổi top, bottom |                                 |
	| --- | --- | --- |
	|	padding     |       Có thể thay đổi cả 4	  |	 	Có thể thay đổi cả 4	    |