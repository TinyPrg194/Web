1. Cấu trúc của Flexbox

    - Thùng chứa cha(flex container)
    - Các phần tử con nằm bên trong(flex items)
    - Một số thuộc tính:

        + main start, main end, cross start, cross end
        + main axis
        + cross axis
        + main size
        + cross size


2. Các thuộc tính của flex container

    - display : định nghĩa một flex container, bắt buộc nếu làm việc với flexbox

    - flex-direction : dùng để chỉ định hướng hiển thị của các item, cho phép thay đổi vị trí của các flex item

        + flex-direction: row  là giá trị mặc định khi sử dụng flexbox, không thực hiện bất kỳ thay đổi nào, chỉ đặt các item từ trái qua phải theo trục chính.
        + flex-direction: row-reverse ngược lại với row, các item sẽ được đặt từ phải qua trái
        + flex-direction: column, lúc này trục chính sẽ đi từ trên xuống dưới vậy nên giờ đây các items sẽ được xếp chồng lên nhau
        + flex-direction:solumn-reverse, các item sẽ được xếp chồng lên nhau nhưng theo chiều ngược lại


    - flex-wrap:dùng để kiểm soát việc bọc các items nằm gọn trong container bao gồm : 

        + nowrap(mặc định)
        + wrap(các item sẽ được bọc gọn trong container)
        + wrap-reverse(ngược lại với wrap)


    - flex-flow: là cách viết rút gọn của flex-direction và flex-wrap với giá trị đầu tiên là flex-direction và giá trị thứ 2 là flex-wrap


    - justify-content : dùng để căn chỉnh vị trí của các items so với truc chính(main axis)

        + flex-start: sẽ đặt item bắt đầu từ main start (và đây cũng là giá trị mặc định)
        + flex-end:sẽ đặt item bắt đầu từ main end
        + center: sẽ đặt tất cả item ở giữa trục main axis
        + space-between: sẽ chia đều khoảng cách thừa và thêm nó vào giữa các item
        +space-around: sẽ chia khoảng cách ở đầu và cuối. Khoảng cách ở đầu và cuối sẽ bằng 1 + nửa khoảng cách ở giữa 2 item với nhau
        + space-evenly: sẽ chia khoảng cách đều khoảng cách giữa các item với item, item và main start, item với main end bằng nhau


    - alighn-items : dùng để xác định cách mà các flex item được đặt trong container dọc theo chiều cross axis

        + align-items: stretch: Chiều dài của item sẽ bằng chiều dài của cross axis.
        + align-items: flex-start: Item được đặt ở điểm bắt đầu của cross start(trên cùng bên trái), và kích thước item không bị thay đổi.
        + align-items: flex-end: Item được đặt ở điểm bắt đầu của cross end(dưới cùng bên trái)
        + align-items: center: Item được đặt ở giữa điểm bắt đầu của cross start và điểm bắt đầu của cross end (ở giữa bên trái)
        + align-items: baseline: Item sẽ được đặt dữ theo các ký tự thuộc item đó. Mục đích chính là căn chỉnh dữa liệu dòng văn bản của các item.


    - align-content : tương tự như justify-content nhưng căn theo trục cros-axis

        + align-content: stretch
        + align-content: flex-start
        + align-content: flex-end
        + align-content: center
        + align-content: space-between
        + align-content: space-around
