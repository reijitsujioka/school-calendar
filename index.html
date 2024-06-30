<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>2024年7月 学校生活カレンダー</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }
        .calendar {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            padding: 20px;
            max-width: 800px;
            width: 100%;
        }
        h1 {
            text-align: center;
            color: #333;
        }
        .grid {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 5px;
        }
        .cell {
            border: 1px solid #ddd;
            padding: 10px;
            text-align: center;
        }
        .header {
            font-weight: bold;
            background-color: #f0f0f0;
        }
        .weekend {
            background-color: #f5f5f5;
        }
        button {
            margin-top: 5px;
            padding: 2px 5px;
            font-size: 12px;
            cursor: pointer;
        }
        .morning { background-color: #e6f3ff; }
        .evening { background-color: #e6e6ff; }
        .late { background-color: #ffe6e6; }
        #summary {
            margin-top: 20px;
            text-align: right;
        }
    </style>
</head>
<body>
    <div class="calendar">
        <h1>2024年7月 学校生活カレンダー</h1>
        <div class="grid" id="calendar"></div>
        <div id="summary"></div>
    </div>

    <script>
        let calendarData = [];

        function initializeCalendarData() {
            const savedData = localStorage.getItem('calendarData');
            if (savedData) {
                calendarData = JSON.parse(savedData);
            } else {
                calendarData = Array(31).fill().map(() => ({morning: false, evening: false, late: false}));
            }
        }

        function saveCalendarData() {
            localStorage.setItem('calendarData', JSON.stringify(calendarData));
        }

        function renderCalendar() {
            const calendar = document.getElementById('calendar');
            calendar.innerHTML = '';
            
            ['日', '月', '火', '水', '木', '金', '土'].forEach(day => {
                const cell = document.createElement('div');
                cell.className = 'cell header';
                cell.textContent = day;
                calendar.appendChild(cell);
            });

            for (let i = 1; i <= 31; i++) {
                const date = new Date(2024, 6, i);
                const cell = document.createElement('div');
                cell.className = `cell ${date.getDay() === 0 || date.getDay() === 6 ? 'weekend' : ''}`;
                
                const dayNumber = document.createElement('div');
                dayNumber.textContent = i;
                cell.appendChild(dayNumber);

                ['morning', 'evening', 'late'].forEach(activity => {
                    const button = document.createElement('button');
                    button.textContent = activity === 'morning' ? '朝練' : activity === 'evening' ? '夕練' : '遅刻';
                    button.onclick = () => toggleActivity(i - 1, activity);
                    button.className = calendarData[i - 1][activity] ? activity : '';
                    cell.appendChild(button);
                });

                calendar.appendChild(cell);
            }

            updateSummary();
        }

        function toggleActivity(day, activity) {
            calendarData[day][activity] = !calendarData[day][activity];
            saveCalendarData();
            renderCalendar();
        }

        function updateSummary() {
            const summary = document.getElementById('summary');
            const counts = calendarData.reduce((acc, day) => {
                if (day.morning) acc.morning++;
                if (day.evening) acc.evening++;
                if (day.late) acc.late++;
                return acc;
            }, {morning: 0, evening: 0, late: 0});

            summary.innerHTML = `
                朝練回数: ${counts.morning} |
                夕練回数: ${counts.evening} |
                遅刻回数: ${counts.late}
            `;
        }

        initializeCalendarData();
        renderCalendar();
    </script>
</body>
</html>
