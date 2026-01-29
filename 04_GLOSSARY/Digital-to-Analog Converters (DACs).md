A **DAC (Digital-to-Analog Converter)** translates digital audio data (0s and 1s) from sources like smartphones, computers, or CDs into a continuous analog signal for speakers and headphones. While built into most devices, dedicated external DACs enhance sound quality by providing more accurate, higher-fidelity signal conversion.

*Need of DAC*
Information exists in real world in analog form. However, we convert them to digital format as the processing speed of a digital computer is much faster and can process data in a matter of micro seconds. It conserves time and helps in processing complex data but humans cannot directly precieve digital data.

In order to understand digital data, it must be converted into an analog domain. 

*How it works*
- **Input:** Receives digital data as a series of binary numbers (0s and 1s). 
- **Conversion:** 
	- Bits are grouped in groups of 8, 16, or 24 bits depending on the native architecture. 
	- Bit weight = $2^n$, where $n$ is the index of the number starting from $0$ to group length - 1. 
	- since the bits can either be $1$ or $0$, it means 
		- bit value of $1$ = $1 * 2 ^ n$
		- bit value of $0$ = $0 * 2 ^ n$
	- then these weights are added together and interpreted as a number. 
	- the numbers are then mapped to a physical range
		- minimum number -> minimum output voltage
		- maximum number -> maximum output voltage 
		- intermediate values scale proportionally
	- Time coordination (when applicable)
		- If the data represents a time-varying signal:
		    - a clock defines **when** each value is applied.
		    - each numeric value is output at a fixed time interval.
			- without timing information, the output represents a static value.
- **Output:** The system produces a continuous physical quantity. 
	- voltage
	- current
	- charges
	- light intensity
	- the exact output depends on the converter and application. 