x64 instruction

	lea : load effective address
	ret : jmp rsp
              add 8, rsp
	rep : rcx 레지스터를 1씩 감소시키면서, 문자열 관련 명령어를 처리한다
	memset, memcpy를 만들 수 있지 않을까?
	STOS : ax를 edi가 가리키는 주소에 넣음
		rep stos byte ptr [EDI] - rcx를 1씩 감소시키면서 ax를 edi가 가리키는 주소에 넣음
	SCAS(scan string) - : AX에 저장되 있는 값과 EDI가 가리키는 곳에 저장되어있는 값을 비교
	strcmp구현 가능
	
Stack
	call func
	local variable save and usage
	func argv delivery(7th arg ~)
