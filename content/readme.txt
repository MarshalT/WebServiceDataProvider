��Ŀ��ַ��https://github.com/iamscottxu/WebServiceDataProvider
�����ļ���https://github.com/iamscottxu/WebServiceDataProvider/blob/master/README.md
���Э�飺https://github.com/iamscottxu/WebServiceDataProvider/blob/master/LICENSE

WebServiceDataProvider��һ�����ڶ�̬����WebService��C#��⣬ʹ�ô���⣬�������Խ�ͨ
�����������������WebService�ṩ�ķ�����������ʹ�ö�̬����Ĵ�����������Щ����������
���ڱ���ǰ��Ӻ�WebService�����ã�ֻ����������⣬��Ϳ�������Ҫʱ����ʹ��
WebService�ṩ�ķ���


����
	Newtonsoft.json >= 11.0.2


���ٿ�ʼ
	�������Ŀ�������������Ϊ��Scottxu.WebServiceDataProvider����NuGet�����������ʹ�á�


���ʹ��
	ֻ��򵥵ļ��д��룬�Ϳ��Ե����κ�WebService��

	ʹ�÷���������
		using Scottxu.WebServiceDataProvider;
		var connection = new Connection("http://xxxx/xxxx.asmx");
		var command = connection.GetMethodCommand("WebService������", "WebService����");
		string returnString = connection.Query();

	ʹ�ö�̬�����C#�������
		using Scottxu.WebServiceDataProvider;
		var connection = new Connection("http://xxxx/xxxx.asmx");
		var command = connection.GetCSharpCommand(
			"var webService = new WebService����();" +
			"return webService.WebService������();" +
		);
		string returnString = connection.Query();


��ϵ����
	������κ�������дIssus��
	Email��xyc0714@aliyun.com

���Э��
MIT License

Copyright (c) 2018 Scott Xu <xyc0714@aliyun.com>

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