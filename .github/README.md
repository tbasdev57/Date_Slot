# @tbasdev57/Date_Slot

Flexible date picker for React. Composable. Customizable. Open Source.

!![Aperçu de l'application](https://github.com/tbasdev57/Date_Slot/blob/main/preview1.png)


## Usage

**Install the package.**

```bash
npm install @tbasdev57/Date_Slot
```

**Compose your calendar.**

```ts
import { Calendar } from '@tbasdev57/Date_Slot';
import { ChevronLeft, ChevronRight } from 'lucide-react';

const MyDatePicker = () => {

	return (
		<Calendar
			className="border p-3"
			mode="single"
			weekStartDay="monday"
			showOutsideDates
		>
			<Calendar.Header>
				<Calendar.Title />
				<div className="space-x-1 flex items-center">
					<Calendar.NavButton direction="previous">
						<ChevronLeft />
					</Calendar.NavButton>
					<Calendar.NavButton direction="next" >
						<ChevronRight />
					</Calendar.NavButton>
				</div>
			</Calendar.Header>
			<Calendar.Content>
				<Calendar.Head />
				<Calendar.Grid
					classNames={ { day: 'h-9 w-9 text-center data-[is-selected=true]:bg-slate-900 data-[is-first=true]:rounded-l-md data-[is-last=true]:rounded-r-md' } }
				/>
			</Calendar.Content>
		</Calendar>
	);
};

export default MyDatePicker;
```

## Documentation

Not available yet.

## License

Under [MIT license](https://github.com/BryanBerger98/datepicker/blob/main/LICENSE.txt).     MIT License

MIT License

Copyright (c) 2024 datepicker by tbasdev57

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
