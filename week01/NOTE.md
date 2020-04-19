# 每周总结可以写在这里
Types

     Undefined, Null, Boolean, String, Symbol, Number,
    and Object.

URI解析

function parseURI(uri){
    let regURI = /^(([^:\/?#]+):)?(\/\/([^\/?#]*))?([^?#]*)(\?([^#]*))?(#(.*))?/
    if(regURI.test(uri)){
        let URIelements = regURI.exec(uri)
        return {
            'Reference':uri,
            'scheme':URIelements[2],
            'authority':URIelements[4],
            'path':URIelements[5],
            'query':URIelements[7],
            'fragment':URIelements[9]
        }
    }else{
        return ''
    }
}

总结
    对知识的掌握 首先要建立知识体系 掌握原理，知其然知其所以然！