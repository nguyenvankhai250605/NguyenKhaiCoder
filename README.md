using System;

class Program
{
    static void Main(string[] args)
    {
        // 1. Chào hỏi và xuất thông báo ra màn hình
        Console.WriteLine("Chào mừng bạn đến với chương trình nhập xuất cơ bản!");
        Console.WriteLine("-------------------------------------------------");

        // 2. Nhập dữ liệu từ người dùng
        Console.Write("Vui lòng nhập tên của bạn: ");
        string name = Console.ReadLine();

        Console.Write("Nhập năm sinh của bạn: ");
        // Console.ReadLine() đọc dữ liệu dưới dạng chuỗi, cần chuyển sang số nguyên để tính toán
        string yearOfBirthString = Console.ReadLine();

        // 3. Xử lý lỗi khi người dùng nhập sai định dạng
        int yearOfBirth;
        bool isParsedSuccessfully = int.TryParse(yearOfBirthString, out yearOfBirth);

        if (isParsedSuccessfully)
        {
            // 4. Tính toán tuổi
            int currentYear = DateTime.Now.Year;
            int age = currentYear - yearOfBirth;

            // 5. Xuất kết quả
            Console.WriteLine("-------------------------------------------------");
            Console.WriteLine("Xin chào, " + name + "!");
            Console.WriteLine("Dựa trên năm sinh của bạn, bạn đã " + age + " tuổi.");
        }
        else
        {
            // Báo lỗi nếu dữ liệu nhập vào không phải là số
            Console.WriteLine("Bạn đã nhập năm sinh không hợp lệ. Vui lòng nhập một số.");
        }

        // 6. Chờ người dùng nhấn phím để kết thúc chương trình
        Console.WriteLine("Nhấn phím bất kỳ để thoát chương trình...");
        Console.ReadKey();
    }
}
