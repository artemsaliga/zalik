# zalik
Саліга Артем КІ-1 1курс

    def analyze_text(file_path):
        try:
            with open(file_path, 'r', encoding='utf-8') as file:
                for line_number, line in enumerate(file, start=1):
                    words = len(line.split())
                    characters = len(line)
                    print(f"Рядок {line_number}: Слів - {words}, Символів - {characters}")
    
        except FileNotFoundError:
            print("Файл не знайдено.")
        except Exception as e:
            print(f"Помилка: {e}")
    
    
    file_path = 'file.txt'
    analyze_text(file_path)
