{"title":"Basic","meta":{"title":"Basic","description":"\n<p>A simple case.</p>\n","order":"0"},"codes":{"jsx":"import { VirtualList } from '@alifd/next';\n\nconst dataSource = [];\n\nconst generateLi = (index = 'index') => {\n    const data = [];\n    if (index % 3 === 0) {\n        return <li key={`key-${index}`} style={{lineHeight: '30px', background: '#5f83ff', color: '#fff'}}>key-{index}</li>;\n    } else {\n        return <li key={`key-${index}`}  style={{lineHeight: '20px'}}>key-{index}</li>;\n    }\n};\n\nfor (let i = 0; i < 1000; i++) {\n    dataSource.push(generateLi(i));\n}\n\nconst demo = (\n    <div className={'virtual-box'}>\n        <VirtualList>\n            {dataSource}\n        </VirtualList>\n    </div>\n);\n\n\nReactDOM.render(demo, mountNode);\n","css":".virtual-box {\n    height: 200px;\n    width: 200px;\n    border: 1px solid #ddd;\n    overflow: auto;\n}\n.virtual-box ul {\n    padding: 0;\n    margin: 0;\n    list-style: none;\n}\n.virtual-box li {\n    padding-left: 10px;\n    border-bottom: 1px solid #333;\n}\n"},"body":"\n````jsx\nimport { VirtualList } from '@alifd/next';\n\nconst dataSource = [];\n\nconst generateLi = (index = 'index') => {\n    const data = [];\n    if (index % 3 === 0) {\n        return <li key={`key-${index}`} style={{lineHeight: '30px', background: '#5f83ff', color: '#fff'}}>key-{index}</li>;\n    } else {\n        return <li key={`key-${index}`}  style={{lineHeight: '20px'}}>key-{index}</li>;\n    }\n};\n\nfor (let i = 0; i < 1000; i++) {\n    dataSource.push(generateLi(i));\n}\n\nconst demo = (\n    <div className={'virtual-box'}>\n        <VirtualList>\n            {dataSource}\n        </VirtualList>\n    </div>\n);\n\n\nReactDOM.render(demo, mountNode);\n````\n\n````css\n.virtual-box {\n    height: 200px;\n    width: 200px;\n    border: 1px solid #ddd;\n    overflow: auto;\n}\n.virtual-box ul {\n    padding: 0;\n    margin: 0;\n    list-style: none;\n}\n.virtual-box li {\n    padding-left: 10px;\n    border-bottom: 1px solid #333;\n}\n````","html":"<script>(function(){'use strict';\n\nvar _next = require('@alifd/next');\n\nvar dataSource = [];\n\nvar generateLi = function generateLi() {\n    var index = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : 'index';\n\n    var data = [];\n    if (index % 3 === 0) {\n        return React.createElement(\n            'li',\n            { key: 'key-' + index, style: { lineHeight: '30px', background: '#5f83ff', color: '#fff' } },\n            'key-',\n            index\n        );\n    } else {\n        return React.createElement(\n            'li',\n            { key: 'key-' + index, style: { lineHeight: '20px' } },\n            'key-',\n            index\n        );\n    }\n};\n\nfor (var i = 0; i < 1000; i++) {\n    dataSource.push(generateLi(i));\n}\n\nvar demo = React.createElement(\n    'div',\n    { className: 'virtual-box' },\n    React.createElement(\n        _next.VirtualList,\n        null,\n        dataSource\n    )\n);\n\nReactDOM.render(demo, mountNode);})()</script><div class=\"highlight\"><pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> VirtualList <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">'@alifd/next'</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> dataSource <span class=\"token operator\">=</span> <span class=\"token punctuation\">[</span><span class=\"token punctuation\">]</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">const</span> generateLi <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span>index <span class=\"token operator\">=</span> <span class=\"token string\">'index'</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n    <span class=\"token keyword\">const</span> data <span class=\"token operator\">=</span> <span class=\"token punctuation\">[</span><span class=\"token punctuation\">]</span><span class=\"token punctuation\">;</span>\n    <span class=\"token keyword\">if</span> <span class=\"token punctuation\">(</span>index <span class=\"token operator\">%</span> <span class=\"token number\">3</span> <span class=\"token operator\">===</span> <span class=\"token number\">0</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">return</span> <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>li</span> <span class=\"token attr-name\">key</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token template-string\"><span class=\"token string\">`key-</span><span class=\"token interpolation\"><span class=\"token interpolation-punctuation punctuation\">${</span>index<span class=\"token interpolation-punctuation punctuation\">}</span></span><span class=\"token string\">`</span></span><span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span>lineHeight<span class=\"token punctuation\">:</span> <span class=\"token string\">'30px'</span><span class=\"token punctuation\">,</span> background<span class=\"token punctuation\">:</span> <span class=\"token string\">'#5f83ff'</span><span class=\"token punctuation\">,</span> color<span class=\"token punctuation\">:</span> <span class=\"token string\">'#fff'</span><span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">key-</span><span class=\"token punctuation\">{</span>index<span class=\"token punctuation\">}</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>li</span><span class=\"token punctuation\">></span></span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span> <span class=\"token keyword\">else</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">return</span> <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>li</span> <span class=\"token attr-name\">key</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token template-string\"><span class=\"token string\">`key-</span><span class=\"token interpolation\"><span class=\"token interpolation-punctuation punctuation\">${</span>index<span class=\"token interpolation-punctuation punctuation\">}</span></span><span class=\"token string\">`</span></span><span class=\"token punctuation\">}</span></span>  <span class=\"token attr-name\">style</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token punctuation\">{</span>lineHeight<span class=\"token punctuation\">:</span> <span class=\"token string\">'20px'</span><span class=\"token punctuation\">}</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">key-</span><span class=\"token punctuation\">{</span>index<span class=\"token punctuation\">}</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>li</span><span class=\"token punctuation\">></span></span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n<span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">for</span> <span class=\"token punctuation\">(</span><span class=\"token keyword\">let</span> i <span class=\"token operator\">=</span> <span class=\"token number\">0</span><span class=\"token punctuation\">;</span> i <span class=\"token operator\">&lt;</span> <span class=\"token number\">1000</span><span class=\"token punctuation\">;</span> i<span class=\"token operator\">++</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n    dataSource<span class=\"token punctuation\">.</span><span class=\"token function\">push</span><span class=\"token punctuation\">(</span><span class=\"token function\">generateLi</span><span class=\"token punctuation\">(</span>i<span class=\"token punctuation\">)</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n<span class=\"token punctuation\">}</span>\n\n<span class=\"token keyword\">const</span> demo <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span>\n    <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span> <span class=\"token attr-name\">className</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token string\">'virtual-box'</span><span class=\"token punctuation\">}</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>VirtualList</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n            </span><span class=\"token punctuation\">{</span>dataSource<span class=\"token punctuation\">}</span><span class=\"token plain-text\">\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>VirtualList</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n    </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span>\n<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n\n\nReactDOM<span class=\"token punctuation\">.</span><span class=\"token function\">render</span><span class=\"token punctuation\">(</span>demo<span class=\"token punctuation\">,</span> mountNode<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span></code></pre></div><style type=\"text/css\">.virtual-box {\n    height: 200px;\n    width: 200px;\n    border: 1px solid #ddd;\n    overflow: auto;\n}\n.virtual-box ul {\n    padding: 0;\n    margin: 0;\n    list-style: none;\n}\n.virtual-box li {\n    padding-left: 10px;\n    border-bottom: 1px solid #333;\n}</style><div class=\"highlight\"><pre class=\"language-css\"><code class=\"language-css\"><span class=\"token selector\">.virtual-box</span> <span class=\"token punctuation\">{</span>\n    <span class=\"token property\">height</span><span class=\"token punctuation\">:</span> 200px<span class=\"token punctuation\">;</span>\n    <span class=\"token property\">width</span><span class=\"token punctuation\">:</span> 200px<span class=\"token punctuation\">;</span>\n    <span class=\"token property\">border</span><span class=\"token punctuation\">:</span> 1px solid #ddd<span class=\"token punctuation\">;</span>\n    <span class=\"token property\">overflow</span><span class=\"token punctuation\">:</span> auto<span class=\"token punctuation\">;</span>\n<span class=\"token punctuation\">}</span>\n<span class=\"token selector\">.virtual-box ul</span> <span class=\"token punctuation\">{</span>\n    <span class=\"token property\">padding</span><span class=\"token punctuation\">:</span> 0<span class=\"token punctuation\">;</span>\n    <span class=\"token property\">margin</span><span class=\"token punctuation\">:</span> 0<span class=\"token punctuation\">;</span>\n    <span class=\"token property\">list-style</span><span class=\"token punctuation\">:</span> none<span class=\"token punctuation\">;</span>\n<span class=\"token punctuation\">}</span>\n<span class=\"token selector\">.virtual-box li</span> <span class=\"token punctuation\">{</span>\n    <span class=\"token property\">padding-left</span><span class=\"token punctuation\">:</span> 10px<span class=\"token punctuation\">;</span>\n    <span class=\"token property\">border-bottom</span><span class=\"token punctuation\">:</span> 1px solid #333<span class=\"token punctuation\">;</span>\n<span class=\"token punctuation\">}</span></code></pre></div>"}