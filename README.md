# api documentation for  [monitor (v0.6.10)](http://lorenwest.github.com/node-monitor/)  [![npm package](https://img.shields.io/npm/v/npmdoc-monitor.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-monitor) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-monitor.svg)](https://travis-ci.org/npmdoc/node-npmdoc-monitor)
#### Runtime monitoring for node.js applications

[![NPM](https://nodei.co/npm/monitor.png?downloads=true)](https://www.npmjs.com/package/monitor)

[![apidoc](https://npmdoc.github.io/node-npmdoc-monitor/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-monitor_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-monitor/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-monitor/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Loren West",
        "email": "open_source@lorenwest.com",
        "url": "https://github.com/lorenwest"
    },
    "bugs": {
        "url": "https://github.com/lorenwest/node-monitor/issues"
    },
    "dependencies": {
        "backbone": "0.9.9",
        "backbone-callbacks": ">=0.1.4 <0.2.0",
        "config": ">=0.4.34 <0.5.0",
        "cron": ">=0.1.3 <0.2.0",
        "socket.io": ">=0.9.10 <0.10.0",
        "socket.io-client": ">=0.9.11 <0.10.0",
        "underscore": ">=1.4.3 <1.5.0"
    },
    "description": "Runtime monitoring for node.js applications",
    "devDependencies": {
        "grunt": "0.3.17"
    },
    "directories": {},
    "dist": {
        "shasum": "c417100bf9dda876dc4146a12c5e852bd8ee08dc",
        "tarball": "https://registry.npmjs.org/monitor/-/monitor-0.6.10.tgz"
    },
    "engines": {
        "node": ">= 0.6.0"
    },
    "homepage": "http://lorenwest.github.com/node-monitor/",
    "keywords": [
        "monitor",
        "node-monitor",
        "remote control",
        "realtime",
        "probe",
        "JMX"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "https://github.com/lorenwest/node-monitor/blob/master/LICENSE"
        }
    ],
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "lorenwest",
            "email": "npm@lorenwest.com"
        }
    ],
    "name": "monitor",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/lorenwest/node-monitor.git"
    },
    "scripts": {
        "start": "node monitor",
        "test": "grunt test"
    },
    "version": "0.6.10"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module monitor](#apidoc.module.monitor)
1.  boolean <span class="apidocSignatureSpan">monitor.</span>commonJS
1.  [function <span class="apidocSignatureSpan">monitor.</span>Backbone.Collection (models, options)](#apidoc.element.monitor.Backbone.Collection)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Backbone.History ()](#apidoc.element.monitor.Backbone.History)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Backbone.Model (attributes, options)](#apidoc.element.monitor.Backbone.Model)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Backbone.Router (options)](#apidoc.element.monitor.Backbone.Router)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Backbone.View (options)](#apidoc.element.monitor.Backbone.View)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Connection ()](#apidoc.element.monitor.Connection)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Connection.List ()](#apidoc.element.monitor.Connection.List)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Cron.CronJob (cronTime, event, oncomplete)](#apidoc.element.monitor.Cron.CronJob)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Cron.CronTime (time)](#apidoc.element.monitor.Cron.CronTime)
1.  [function <span class="apidocSignatureSpan">monitor.</span>DataModelProbe ()](#apidoc.element.monitor.DataModelProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>DataModelProbe.List ()](#apidoc.element.monitor.DataModelProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.</span>FileProbe ()](#apidoc.element.monitor.FileProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>InspectProbe ()](#apidoc.element.monitor.InspectProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>List ()](#apidoc.element.monitor.List)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Log (module)](#apidoc.element.monitor.Log)
1.  [function <span class="apidocSignatureSpan">monitor.</span>LogProbe ()](#apidoc.element.monitor.LogProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>PollingProbe ()](#apidoc.element.monitor.PollingProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Probe ()](#apidoc.element.monitor.Probe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>ProcessProbe ()](#apidoc.element.monitor.ProcessProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>RecipeProbe ()](#apidoc.element.monitor.RecipeProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>ReplProbe ()](#apidoc.element.monitor.ReplProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Router ()](#apidoc.element.monitor.Router)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Server ()](#apidoc.element.monitor.Server)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Server.List ()](#apidoc.element.monitor.Server.List)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Stat (module)](#apidoc.element.monitor.Stat)
1.  [function <span class="apidocSignatureSpan">monitor.</span>StatProbe ()](#apidoc.element.monitor.StatProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>StreamProbe ()](#apidoc.element.monitor.StreamProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Sync (className, options)](#apidoc.element.monitor.Sync)
1.  [function <span class="apidocSignatureSpan">monitor.</span>SyncProbe ()](#apidoc.element.monitor.SyncProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>SyncProbe.FileSyncProbe ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>_ (obj)](#apidoc.element.monitor._)
1.  [function <span class="apidocSignatureSpan">monitor.</span>deepCopy (value, depth)](#apidoc.element.monitor.deepCopy)
1.  [function <span class="apidocSignatureSpan">monitor.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.extend)
1.  [function <span class="apidocSignatureSpan">monitor.</span>generateUniqueCollectionId (collection, prefix)](#apidoc.element.monitor.generateUniqueCollectionId)
1.  [function <span class="apidocSignatureSpan">monitor.</span>generateUniqueId ()](#apidoc.element.monitor.generateUniqueId)
1.  [function <span class="apidocSignatureSpan">monitor.</span>getLogger (module)](#apidoc.element.monitor.getLogger)
1.  [function <span class="apidocSignatureSpan">monitor.</span>getRouter ()](#apidoc.element.monitor.getRouter)
1.  [function <span class="apidocSignatureSpan">monitor.</span>getStatLogger (module)](#apidoc.element.monitor.getStatLogger)
1.  [function <span class="apidocSignatureSpan">monitor.</span>setLoggerClass (LoggerClass)](#apidoc.element.monitor.setLoggerClass)
1.  [function <span class="apidocSignatureSpan">monitor.</span>setStatLoggerClass (StatLoggerClass)](#apidoc.element.monitor.setStatLoggerClass)
1.  [function <span class="apidocSignatureSpan">monitor.</span>start (options, callback)](#apidoc.element.monitor.start)
1.  [function <span class="apidocSignatureSpan">monitor.</span>stop (callback)](#apidoc.element.monitor.stop)
1.  [function <span class="apidocSignatureSpan">monitor.</span>stringify (value, depth, indent)](#apidoc.element.monitor.stringify)
1.  [function <span class="apidocSignatureSpan">monitor.</span>toServerString (monitorJSON)](#apidoc.element.monitor.toServerString)
1.  object <span class="apidocSignatureSpan">monitor.</span>Backbone
1.  object <span class="apidocSignatureSpan">monitor.</span>Backbone.Collection.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Backbone.Events
1.  object <span class="apidocSignatureSpan">monitor.</span>Backbone.History.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Backbone.Router.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Backbone.View.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Backbone.history
1.  object <span class="apidocSignatureSpan">monitor.</span>Config
1.  object <span class="apidocSignatureSpan">monitor.</span>Connection.List.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Connection.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Cron
1.  object <span class="apidocSignatureSpan">monitor.</span>Cron.CronJob.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Cron.CronTime.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>DataModelProbe.List.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>DataModelProbe.classes
1.  object <span class="apidocSignatureSpan">monitor.</span>DataModelProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>FileProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>InspectProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>List.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Log._events
1.  object <span class="apidocSignatureSpan">monitor.</span>Log.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>LogProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>PollingProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Probe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>ProcessProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>RecipeProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>ReplProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Router.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Server.List.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Server.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>Stat.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>StatProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>StreamProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>SyncProbe.FileSyncProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>SyncProbe.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>_.prototype
1.  object <span class="apidocSignatureSpan">monitor.</span>__super__

#### [module monitor.Backbone](#apidoc.module.monitor.Backbone)
1.  boolean <span class="apidocSignatureSpan">monitor.Backbone.</span>emulateHTTP
1.  boolean <span class="apidocSignatureSpan">monitor.Backbone.</span>emulateJSON
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>Collection (models, options)](#apidoc.element.monitor.Backbone.Collection)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>History ()](#apidoc.element.monitor.Backbone.History)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>Model (attributes, options)](#apidoc.element.monitor.Backbone.Model)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>Router (options)](#apidoc.element.monitor.Backbone.Router)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>View (options)](#apidoc.element.monitor.Backbone.View)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>ajax ()](#apidoc.element.monitor.Backbone.ajax)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.bind)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.listenTo)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>noConflict ()](#apidoc.element.monitor.Backbone.noConflict)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.off)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.on)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.once)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.stopListening)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>sync (method, model, options)](#apidoc.element.monitor.Backbone.sync)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>trigger (name)](#apidoc.element.monitor.Backbone.trigger)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.unbind)
1.  object <span class="apidocSignatureSpan">monitor.Backbone.</span>Events
1.  object <span class="apidocSignatureSpan">monitor.Backbone.</span>history
1.  string <span class="apidocSignatureSpan">monitor.Backbone.</span>VERSION

#### [module monitor.Backbone.Collection](#apidoc.module.monitor.Backbone.Collection)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>Collection (models, options)](#apidoc.element.monitor.Backbone.Collection.Collection)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.Collection.extend)

#### [module monitor.Backbone.Collection.prototype](#apidoc.module.monitor.Backbone.Collection.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>_onModelEvent (event, model, collection, options)](#apidoc.element.monitor.Backbone.Collection.prototype._onModelEvent)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>_prepareModel (attrs, options)](#apidoc.element.monitor.Backbone.Collection.prototype._prepareModel)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>_removeReference (model)](#apidoc.element.monitor.Backbone.Collection.prototype._removeReference)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>_reset ()](#apidoc.element.monitor.Backbone.Collection.prototype._reset)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>add (models, options)](#apidoc.element.monitor.Backbone.Collection.prototype.add)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>all ()](#apidoc.element.monitor.Backbone.Collection.prototype.all)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>any ()](#apidoc.element.monitor.Backbone.Collection.prototype.any)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>at (index)](#apidoc.element.monitor.Backbone.Collection.prototype.at)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.bind)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>chain ()](#apidoc.element.monitor.Backbone.Collection.prototype.chain)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>clone ()](#apidoc.element.monitor.Backbone.Collection.prototype.clone)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>collect ()](#apidoc.element.monitor.Backbone.Collection.prototype.collect)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>contains ()](#apidoc.element.monitor.Backbone.Collection.prototype.contains)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>countBy (value, context)](#apidoc.element.monitor.Backbone.Collection.prototype.countBy)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>create (model, options)](#apidoc.element.monitor.Backbone.Collection.prototype.create)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>detect ()](#apidoc.element.monitor.Backbone.Collection.prototype.detect)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>each ()](#apidoc.element.monitor.Backbone.Collection.prototype.each)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>every ()](#apidoc.element.monitor.Backbone.Collection.prototype.every)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>fetch ()](#apidoc.element.monitor.Backbone.Collection.prototype.fetch)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>filter ()](#apidoc.element.monitor.Backbone.Collection.prototype.filter)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>find ()](#apidoc.element.monitor.Backbone.Collection.prototype.find)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>first ()](#apidoc.element.monitor.Backbone.Collection.prototype.first)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>foldl ()](#apidoc.element.monitor.Backbone.Collection.prototype.foldl)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>foldr ()](#apidoc.element.monitor.Backbone.Collection.prototype.foldr)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>forEach ()](#apidoc.element.monitor.Backbone.Collection.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>get (obj)](#apidoc.element.monitor.Backbone.Collection.prototype.get)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>groupBy (value, context)](#apidoc.element.monitor.Backbone.Collection.prototype.groupBy)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>head ()](#apidoc.element.monitor.Backbone.Collection.prototype.head)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>include ()](#apidoc.element.monitor.Backbone.Collection.prototype.include)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>indexOf ()](#apidoc.element.monitor.Backbone.Collection.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>initial ()](#apidoc.element.monitor.Backbone.Collection.prototype.initial)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>initialize ()](#apidoc.element.monitor.Backbone.Collection.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>inject ()](#apidoc.element.monitor.Backbone.Collection.prototype.inject)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>invoke ()](#apidoc.element.monitor.Backbone.Collection.prototype.invoke)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>isEmpty ()](#apidoc.element.monitor.Backbone.Collection.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>last ()](#apidoc.element.monitor.Backbone.Collection.prototype.last)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>lastIndexOf ()](#apidoc.element.monitor.Backbone.Collection.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.Collection.prototype.listenTo)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>map ()](#apidoc.element.monitor.Backbone.Collection.prototype.map)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>max ()](#apidoc.element.monitor.Backbone.Collection.prototype.max)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>min ()](#apidoc.element.monitor.Backbone.Collection.prototype.min)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>model (attributes, options)](#apidoc.element.monitor.Backbone.Collection.prototype.model)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.off)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.on)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.once)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>parse (resp)](#apidoc.element.monitor.Backbone.Collection.prototype.parse)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>pluck (attr)](#apidoc.element.monitor.Backbone.Collection.prototype.pluck)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>pop (options)](#apidoc.element.monitor.Backbone.Collection.prototype.pop)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>push (model, options)](#apidoc.element.monitor.Backbone.Collection.prototype.push)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>reduce ()](#apidoc.element.monitor.Backbone.Collection.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>reduceRight ()](#apidoc.element.monitor.Backbone.Collection.prototype.reduceRight)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>reject ()](#apidoc.element.monitor.Backbone.Collection.prototype.reject)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>remove (models, options)](#apidoc.element.monitor.Backbone.Collection.prototype.remove)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>reset (models, options)](#apidoc.element.monitor.Backbone.Collection.prototype.reset)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>rest ()](#apidoc.element.monitor.Backbone.Collection.prototype.rest)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>select ()](#apidoc.element.monitor.Backbone.Collection.prototype.select)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>shift (options)](#apidoc.element.monitor.Backbone.Collection.prototype.shift)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>shuffle ()](#apidoc.element.monitor.Backbone.Collection.prototype.shuffle)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>size ()](#apidoc.element.monitor.Backbone.Collection.prototype.size)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>slice (begin, end)](#apidoc.element.monitor.Backbone.Collection.prototype.slice)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>some ()](#apidoc.element.monitor.Backbone.Collection.prototype.some)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>sort (options)](#apidoc.element.monitor.Backbone.Collection.prototype.sort)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>sortBy (value, context)](#apidoc.element.monitor.Backbone.Collection.prototype.sortBy)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>sortedIndex ()](#apidoc.element.monitor.Backbone.Collection.prototype.sortedIndex)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.Collection.prototype.stopListening)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>sync ()](#apidoc.element.monitor.Backbone.Collection.prototype.sync)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>tail ()](#apidoc.element.monitor.Backbone.Collection.prototype.tail)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>take ()](#apidoc.element.monitor.Backbone.Collection.prototype.take)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>toArray ()](#apidoc.element.monitor.Backbone.Collection.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>toJSON (options)](#apidoc.element.monitor.Backbone.Collection.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>trigger (name)](#apidoc.element.monitor.Backbone.Collection.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.unbind)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>unshift (model, options)](#apidoc.element.monitor.Backbone.Collection.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>update (models, options)](#apidoc.element.monitor.Backbone.Collection.prototype.update)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>where (attrs)](#apidoc.element.monitor.Backbone.Collection.prototype.where)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>without ()](#apidoc.element.monitor.Backbone.Collection.prototype.without)

#### [module monitor.Backbone.Events](#apidoc.module.monitor.Backbone.Events)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.Events.bind)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.Events.listenTo)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.Events.off)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.Events.on)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.Events.once)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.Events.stopListening)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>trigger (name)](#apidoc.element.monitor.Backbone.Events.trigger)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.Events.unbind)

#### [module monitor.Backbone.History](#apidoc.module.monitor.Backbone.History)
1.  boolean <span class="apidocSignatureSpan">monitor.Backbone.History.</span>started
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>History ()](#apidoc.element.monitor.Backbone.History.History)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.History.extend)

#### [module monitor.Backbone.History.prototype](#apidoc.module.monitor.Backbone.History.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>_updateHash (location, fragment, replace)](#apidoc.element.monitor.Backbone.History.prototype._updateHash)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.bind)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>checkUrl (e)](#apidoc.element.monitor.Backbone.History.prototype.checkUrl)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>getFragment (fragment, forcePushState)](#apidoc.element.monitor.Backbone.History.prototype.getFragment)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>getHash (window)](#apidoc.element.monitor.Backbone.History.prototype.getHash)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.History.prototype.listenTo)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>loadUrl (fragmentOverride)](#apidoc.element.monitor.Backbone.History.prototype.loadUrl)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>navigate (fragment, options)](#apidoc.element.monitor.Backbone.History.prototype.navigate)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.off)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.on)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.once)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>route (route, callback)](#apidoc.element.monitor.Backbone.History.prototype.route)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>start (options)](#apidoc.element.monitor.Backbone.History.prototype.start)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>stop ()](#apidoc.element.monitor.Backbone.History.prototype.stop)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.History.prototype.stopListening)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>trigger (name)](#apidoc.element.monitor.Backbone.History.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.unbind)
1.  number <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>interval

#### [module monitor.Backbone.Model](#apidoc.module.monitor.Backbone.Model)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>Model (attributes, options)](#apidoc.element.monitor.Backbone.Model.Model)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Model.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.Model.extend)

#### [module monitor.Backbone.Router](#apidoc.module.monitor.Backbone.Router)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>Router (options)](#apidoc.element.monitor.Backbone.Router.Router)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.Router.extend)

#### [module monitor.Backbone.Router.prototype](#apidoc.module.monitor.Backbone.Router.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>_bindRoutes ()](#apidoc.element.monitor.Backbone.Router.prototype._bindRoutes)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>_extractParameters (route, fragment)](#apidoc.element.monitor.Backbone.Router.prototype._extractParameters)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>_routeToRegExp (route)](#apidoc.element.monitor.Backbone.Router.prototype._routeToRegExp)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.bind)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>initialize ()](#apidoc.element.monitor.Backbone.Router.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.Router.prototype.listenTo)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>navigate (fragment, options)](#apidoc.element.monitor.Backbone.Router.prototype.navigate)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.off)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.on)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.once)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>route (route, name, callback)](#apidoc.element.monitor.Backbone.Router.prototype.route)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.Router.prototype.stopListening)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>trigger (name)](#apidoc.element.monitor.Backbone.Router.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.unbind)

#### [module monitor.Backbone.View](#apidoc.module.monitor.Backbone.View)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.</span>View (options)](#apidoc.element.monitor.Backbone.View.View)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.View.extend)

#### [module monitor.Backbone.View.prototype](#apidoc.module.monitor.Backbone.View.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>_configure (options)](#apidoc.element.monitor.Backbone.View.prototype._configure)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>_ensureElement ()](#apidoc.element.monitor.Backbone.View.prototype._ensureElement)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.bind)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>delegateEvents (events)](#apidoc.element.monitor.Backbone.View.prototype.delegateEvents)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>initialize ()](#apidoc.element.monitor.Backbone.View.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.View.prototype.listenTo)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>make (tagName, attributes, content)](#apidoc.element.monitor.Backbone.View.prototype.make)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.off)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.on)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.once)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>remove ()](#apidoc.element.monitor.Backbone.View.prototype.remove)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>render ()](#apidoc.element.monitor.Backbone.View.prototype.render)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>setElement (element, delegate)](#apidoc.element.monitor.Backbone.View.prototype.setElement)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.View.prototype.stopListening)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>trigger (name)](#apidoc.element.monitor.Backbone.View.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.unbind)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>undelegateEvents ()](#apidoc.element.monitor.Backbone.View.prototype.undelegateEvents)
1.  string <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>tagName

#### [module monitor.Backbone.history](#apidoc.module.monitor.Backbone.history)
1.  [function <span class="apidocSignatureSpan">monitor.Backbone.history.</span>checkUrl ()](#apidoc.element.monitor.Backbone.history.checkUrl)
1.  object <span class="apidocSignatureSpan">monitor.Backbone.history.</span>handlers

#### [module monitor.Connection](#apidoc.module.monitor.Connection)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Connection ()](#apidoc.element.monitor.Connection.Connection)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.</span>List ()](#apidoc.element.monitor.Connection.List)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Connection.extend)
1.  object <span class="apidocSignatureSpan">monitor.Connection.</span>__super__

#### [module monitor.Connection.List](#apidoc.module.monitor.Connection.List)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.</span>List ()](#apidoc.element.monitor.Connection.List.List)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.List.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Connection.List.extend)
1.  object <span class="apidocSignatureSpan">monitor.Connection.List.</span>__super__

#### [module monitor.Connection.List.prototype](#apidoc.module.monitor.Connection.List.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.List.prototype.</span>constructor ()](#apidoc.element.monitor.Connection.List.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.List.prototype.</span>model ()](#apidoc.element.monitor.Connection.List.prototype.model)

#### [module monitor.Connection.prototype](#apidoc.module.monitor.Connection.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>addEvent (eventName, handler)](#apidoc.element.monitor.Connection.prototype.addEvent)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>bindConnectionEvents ()](#apidoc.element.monitor.Connection.prototype.bindConnectionEvents)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>connect ()](#apidoc.element.monitor.Connection.prototype.connect)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>constructor ()](#apidoc.element.monitor.Connection.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>disconnect (reason)](#apidoc.element.monitor.Connection.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>emit ()](#apidoc.element.monitor.Connection.prototype.emit)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>initialize (params)](#apidoc.element.monitor.Connection.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>isThisHost (hostName)](#apidoc.element.monitor.Connection.prototype.isThisHost)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>ping (callback)](#apidoc.element.monitor.Connection.prototype.ping)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>probeConnect (monitorJSON, callback)](#apidoc.element.monitor.Connection.prototype.probeConnect)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>probeControl (params, callback)](#apidoc.element.monitor.Connection.prototype.probeControl)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>probeDisconnect (params, callback)](#apidoc.element.monitor.Connection.prototype.probeDisconnect)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>removeAllEvents ()](#apidoc.element.monitor.Connection.prototype.removeAllEvents)
1.  [function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>removeEvent (eventName)](#apidoc.element.monitor.Connection.prototype.removeEvent)
1.  object <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>defaults

#### [module monitor.Cron](#apidoc.module.monitor.Cron)
1.  [function <span class="apidocSignatureSpan">monitor.Cron.</span>CronJob (cronTime, event, oncomplete)](#apidoc.element.monitor.Cron.CronJob)
1.  [function <span class="apidocSignatureSpan">monitor.Cron.</span>CronTime (time)](#apidoc.element.monitor.Cron.CronTime)

#### [module monitor.Cron.CronJob](#apidoc.module.monitor.Cron.CronJob)
1.  [function <span class="apidocSignatureSpan">monitor.Cron.</span>CronJob (cronTime, event, oncomplete)](#apidoc.element.monitor.Cron.CronJob.CronJob)

#### [module monitor.Cron.CronJob.prototype](#apidoc.module.monitor.Cron.CronJob.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Cron.CronJob.prototype.</span>addEvent (event)](#apidoc.element.monitor.Cron.CronJob.prototype.addEvent)
1.  [function <span class="apidocSignatureSpan">monitor.Cron.CronJob.prototype.</span>clock ()](#apidoc.element.monitor.Cron.CronJob.prototype.clock)
1.  [function <span class="apidocSignatureSpan">monitor.Cron.CronJob.prototype.</span>runEvents ()](#apidoc.element.monitor.Cron.CronJob.prototype.runEvents)

#### [module monitor.Cron.CronTime](#apidoc.module.monitor.Cron.CronTime)
1.  [function <span class="apidocSignatureSpan">monitor.Cron.</span>CronTime (time)](#apidoc.element.monitor.Cron.CronTime.CronTime)

#### [module monitor.Cron.CronTime.prototype](#apidoc.module.monitor.Cron.CronTime.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Cron.CronTime.prototype.</span>_parse ()](#apidoc.element.monitor.Cron.CronTime.prototype._parse)
1.  [function <span class="apidocSignatureSpan">monitor.Cron.CronTime.prototype.</span>_parseField (field, type, constraints)](#apidoc.element.monitor.Cron.CronTime.prototype._parseField)

#### [module monitor.DataModelProbe](#apidoc.module.monitor.DataModelProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>DataModelProbe ()](#apidoc.element.monitor.DataModelProbe.DataModelProbe)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.</span>List ()](#apidoc.element.monitor.DataModelProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.</span>extend (params)](#apidoc.element.monitor.DataModelProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.DataModelProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.DataModelProbe.</span>classes

#### [module monitor.DataModelProbe.List](#apidoc.module.monitor.DataModelProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.</span>List ()](#apidoc.element.monitor.DataModelProbe.List.List)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.List.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.DataModelProbe.List.extend)
1.  object <span class="apidocSignatureSpan">monitor.DataModelProbe.List.</span>__super__

#### [module monitor.DataModelProbe.List.prototype](#apidoc.module.monitor.DataModelProbe.List.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.List.prototype.</span>constructor ()](#apidoc.element.monitor.DataModelProbe.List.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.List.prototype.</span>model ()](#apidoc.element.monitor.DataModelProbe.List.prototype.model)

#### [module monitor.DataModelProbe.classes](#apidoc.module.monitor.DataModelProbe.classes)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>DataModel ()](#apidoc.element.monitor.DataModelProbe.classes.DataModel)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>File ()](#apidoc.element.monitor.DataModelProbe.classes.File)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>FileSyncProbe ()](#apidoc.element.monitor.DataModelProbe.classes.FileSyncProbe)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Inspect ()](#apidoc.element.monitor.DataModelProbe.classes.Inspect)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Log ()](#apidoc.element.monitor.DataModelProbe.classes.Log)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Process ()](#apidoc.element.monitor.DataModelProbe.classes.Process)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Recipe ()](#apidoc.element.monitor.DataModelProbe.classes.Recipe)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Repl ()](#apidoc.element.monitor.DataModelProbe.classes.Repl)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Stat ()](#apidoc.element.monitor.DataModelProbe.classes.Stat)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Sync ()](#apidoc.element.monitor.DataModelProbe.classes.Sync)

#### [module monitor.DataModelProbe.prototype](#apidoc.module.monitor.DataModelProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.DataModelProbe.prototype.</span>constructor ()](#apidoc.element.monitor.DataModelProbe.prototype.constructor)
1.  string <span class="apidocSignatureSpan">monitor.DataModelProbe.prototype.</span>probeClass
1.  string <span class="apidocSignatureSpan">monitor.DataModelProbe.prototype.</span>writableAttributes

#### [module monitor.FileProbe](#apidoc.module.monitor.FileProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>FileProbe ()](#apidoc.element.monitor.FileProbe.FileProbe)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.</span>List ()](#apidoc.element.monitor.FileProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.</span>extend (params)](#apidoc.element.monitor.FileProbe.extend)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.</span>getRootPath ()](#apidoc.element.monitor.FileProbe.getRootPath)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.</span>mkdir_r (dirname, mode, callback)](#apidoc.element.monitor.FileProbe.mkdir_r)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.</span>rm_rf (path, callback)](#apidoc.element.monitor.FileProbe.rm_rf)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.</span>setRootPath (rootPath)](#apidoc.element.monitor.FileProbe.setRootPath)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.</span>tail ()](#apidoc.element.monitor.FileProbe.tail)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.</span>watch (path, options, callback)](#apidoc.element.monitor.FileProbe.watch)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.</span>watchLoad (path, options, callback)](#apidoc.element.monitor.FileProbe.watchLoad)
1.  object <span class="apidocSignatureSpan">monitor.FileProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.FileProbe.</span>classes

#### [module monitor.FileProbe.prototype](#apidoc.module.monitor.FileProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.prototype.</span>constructor ()](#apidoc.element.monitor.FileProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.FileProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.FileProbe.prototype.</span>release ()](#apidoc.element.monitor.FileProbe.prototype.release)
1.  object <span class="apidocSignatureSpan">monitor.FileProbe.prototype.</span>defaults
1.  string <span class="apidocSignatureSpan">monitor.FileProbe.prototype.</span>probeClass

#### [module monitor.InspectProbe](#apidoc.module.monitor.InspectProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>InspectProbe ()](#apidoc.element.monitor.InspectProbe.InspectProbe)
1.  [function <span class="apidocSignatureSpan">monitor.InspectProbe.</span>List ()](#apidoc.element.monitor.InspectProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.InspectProbe.</span>extend (params)](#apidoc.element.monitor.InspectProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.InspectProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.InspectProbe.</span>classes

#### [module monitor.InspectProbe.prototype](#apidoc.module.monitor.InspectProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>_evaluate (expression)](#apidoc.element.monitor.InspectProbe.prototype._evaluate)
1.  [function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>constructor ()](#apidoc.element.monitor.InspectProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>eval_control (expression, depth)](#apidoc.element.monitor.InspectProbe.prototype.eval_control)
1.  [function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>initialize (initParams)](#apidoc.element.monitor.InspectProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>poll ()](#apidoc.element.monitor.InspectProbe.prototype.poll)
1.  [function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>release ()](#apidoc.element.monitor.InspectProbe.prototype.release)
1.  [function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>set_control (attrs, callback)](#apidoc.element.monitor.InspectProbe.prototype.set_control)
1.  object <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>writableAttributes
1.  string <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>probeClass

#### [module monitor.List](#apidoc.module.monitor.List)
1.  [function <span class="apidocSignatureSpan">monitor.</span>List ()](#apidoc.element.monitor.List.List)
1.  [function <span class="apidocSignatureSpan">monitor.List.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.List.extend)
1.  object <span class="apidocSignatureSpan">monitor.List.</span>__super__

#### [module monitor.List.prototype](#apidoc.module.monitor.List.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.List.prototype.</span>constructor ()](#apidoc.element.monitor.List.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.List.prototype.</span>model ()](#apidoc.element.monitor.List.prototype.model)

#### [module monitor.Log](#apidoc.module.monitor.Log)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Log (module)](#apidoc.element.monitor.Log.Log)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>_emit (type, module, name, args)](#apidoc.element.monitor.Log._emit)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>addListener (type, listener)](#apidoc.element.monitor.Log.addListener)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>console (type, module, name)](#apidoc.element.monitor.Log.console)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>emit (type)](#apidoc.element.monitor.Log.emit)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>eventNames ()](#apidoc.element.monitor.Log.eventNames)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>getMaxListeners ()](#apidoc.element.monitor.Log.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>listenerCount (type)](#apidoc.element.monitor.Log.listenerCount)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>listeners (type)](#apidoc.element.monitor.Log.listeners)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>on (type, listener)](#apidoc.element.monitor.Log.on)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>once (type, listener)](#apidoc.element.monitor.Log.once)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>prependListener (type, listener)](#apidoc.element.monitor.Log.prependListener)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>prependOnceListener (type, listener)](#apidoc.element.monitor.Log.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>removeAllListeners (type)](#apidoc.element.monitor.Log.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>removeListener (type, listener)](#apidoc.element.monitor.Log.removeListener)
1.  [function <span class="apidocSignatureSpan">monitor.Log.</span>setMaxListeners (n)](#apidoc.element.monitor.Log.setMaxListeners)
1.  number <span class="apidocSignatureSpan">monitor.Log.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">monitor.Log.</span>_events
1.  object <span class="apidocSignatureSpan">monitor.Log.</span>eventRegex
1.  undefined <span class="apidocSignatureSpan">monitor.Log.</span>domain

#### [module monitor.Log._events](#apidoc.module.monitor.Log._events)

#### [module monitor.Log.prototype](#apidoc.module.monitor.Log.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>debug (name)](#apidoc.element.monitor.Log.prototype.debug)
1.  [function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>error (name)](#apidoc.element.monitor.Log.prototype.error)
1.  [function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>fatal (name)](#apidoc.element.monitor.Log.prototype.fatal)
1.  [function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>info (name)](#apidoc.element.monitor.Log.prototype.info)
1.  [function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>trace (name)](#apidoc.element.monitor.Log.prototype.trace)
1.  [function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>warn (name)](#apidoc.element.monitor.Log.prototype.warn)

#### [module monitor.LogProbe](#apidoc.module.monitor.LogProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>LogProbe ()](#apidoc.element.monitor.LogProbe.LogProbe)
1.  [function <span class="apidocSignatureSpan">monitor.LogProbe.</span>List ()](#apidoc.element.monitor.LogProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.LogProbe.</span>extend (params)](#apidoc.element.monitor.LogProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.LogProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.LogProbe.</span>classes

#### [module monitor.LogProbe.prototype](#apidoc.module.monitor.LogProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.LogProbe.prototype.</span>constructor ()](#apidoc.element.monitor.LogProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.LogProbe.prototype.</span>initialize ()](#apidoc.element.monitor.LogProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.LogProbe.prototype.</span>release ()](#apidoc.element.monitor.LogProbe.prototype.release)
1.  object <span class="apidocSignatureSpan">monitor.LogProbe.prototype.</span>defaults
1.  string <span class="apidocSignatureSpan">monitor.LogProbe.prototype.</span>probeClass

#### [module monitor.PollingProbe](#apidoc.module.monitor.PollingProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>PollingProbe ()](#apidoc.element.monitor.PollingProbe.PollingProbe)
1.  [function <span class="apidocSignatureSpan">monitor.PollingProbe.</span>List ()](#apidoc.element.monitor.PollingProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.PollingProbe.</span>extend (params)](#apidoc.element.monitor.PollingProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.PollingProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.PollingProbe.</span>classes

#### [module monitor.PollingProbe.prototype](#apidoc.module.monitor.PollingProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.PollingProbe.prototype.</span>constructor ()](#apidoc.element.monitor.PollingProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.PollingProbe.prototype.</span>initialize ()](#apidoc.element.monitor.PollingProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.PollingProbe.prototype.</span>release ()](#apidoc.element.monitor.PollingProbe.prototype.release)
1.  object <span class="apidocSignatureSpan">monitor.PollingProbe.prototype.</span>defaults

#### [module monitor.Probe](#apidoc.module.monitor.Probe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Probe ()](#apidoc.element.monitor.Probe.Probe)
1.  [function <span class="apidocSignatureSpan">monitor.Probe.</span>List ()](#apidoc.element.monitor.Probe.List)
1.  [function <span class="apidocSignatureSpan">monitor.Probe.</span>extend (params)](#apidoc.element.monitor.Probe.extend)
1.  object <span class="apidocSignatureSpan">monitor.Probe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.Probe.</span>classes

#### [module monitor.Probe.prototype](#apidoc.module.monitor.Probe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>constructor ()](#apidoc.element.monitor.Probe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.Probe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>onControl (name, params, callback)](#apidoc.element.monitor.Probe.prototype.onControl)
1.  [function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>ping_control (params, callback)](#apidoc.element.monitor.Probe.prototype.ping_control)
1.  [function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>release ()](#apidoc.element.monitor.Probe.prototype.release)
1.  [function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>set_control (attrs, callback)](#apidoc.element.monitor.Probe.prototype.set_control)
1.  object <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>defaults

#### [module monitor.ProcessProbe](#apidoc.module.monitor.ProcessProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>ProcessProbe ()](#apidoc.element.monitor.ProcessProbe.ProcessProbe)
1.  [function <span class="apidocSignatureSpan">monitor.ProcessProbe.</span>List ()](#apidoc.element.monitor.ProcessProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.ProcessProbe.</span>extend (params)](#apidoc.element.monitor.ProcessProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.ProcessProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.ProcessProbe.</span>classes

#### [module monitor.ProcessProbe.prototype](#apidoc.module.monitor.ProcessProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.ProcessProbe.prototype.</span>constructor ()](#apidoc.element.monitor.ProcessProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.ProcessProbe.prototype.</span>poll ()](#apidoc.element.monitor.ProcessProbe.prototype.poll)
1.  string <span class="apidocSignatureSpan">monitor.ProcessProbe.prototype.</span>probeClass

#### [module monitor.RecipeProbe](#apidoc.module.monitor.RecipeProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>RecipeProbe ()](#apidoc.element.monitor.RecipeProbe.RecipeProbe)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.</span>List ()](#apidoc.element.monitor.RecipeProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.</span>extend (params)](#apidoc.element.monitor.RecipeProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.RecipeProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.RecipeProbe.</span>classes

#### [module monitor.RecipeProbe.prototype](#apidoc.module.monitor.RecipeProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>bringLocal (context)](#apidoc.element.monitor.RecipeProbe.prototype.bringLocal)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>connectListeners (connect)](#apidoc.element.monitor.RecipeProbe.prototype.connectListeners)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>constructor ()](#apidoc.element.monitor.RecipeProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.RecipeProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>onTrigger ()](#apidoc.element.monitor.RecipeProbe.prototype.onTrigger)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>release ()](#apidoc.element.monitor.RecipeProbe.prototype.release)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>run (context)](#apidoc.element.monitor.RecipeProbe.prototype.run)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>run_control (params, callback)](#apidoc.element.monitor.RecipeProbe.prototype.run_control)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>start_control (params, callback)](#apidoc.element.monitor.RecipeProbe.prototype.start_control)
1.  [function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>stop_control (params, callback)](#apidoc.element.monitor.RecipeProbe.prototype.stop_control)
1.  object <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>defaults
1.  object <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>writableAttributes
1.  string <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>probeClass

#### [module monitor.ReplProbe](#apidoc.module.monitor.ReplProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>ReplProbe ()](#apidoc.element.monitor.ReplProbe.ReplProbe)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.</span>List ()](#apidoc.element.monitor.ReplProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.</span>extend (params)](#apidoc.element.monitor.ReplProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.ReplProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.ReplProbe.</span>classes

#### [module monitor.ReplProbe.prototype](#apidoc.module.monitor.ReplProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>_output (str)](#apidoc.element.monitor.ReplProbe.prototype._output)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>_runShellCmd (command)](#apidoc.element.monitor.ReplProbe.prototype._runShellCmd)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>autocomplete_control (params, callback)](#apidoc.element.monitor.ReplProbe.prototype.autocomplete_control)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>constructor ()](#apidoc.element.monitor.ReplProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.ReplProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>input_control (params, callback)](#apidoc.element.monitor.ReplProbe.prototype.input_control)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>release ()](#apidoc.element.monitor.ReplProbe.prototype.release)
1.  [function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>sh_control (params, callback)](#apidoc.element.monitor.ReplProbe.prototype.sh_control)
1.  object <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>defaults
1.  string <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>description
1.  string <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>probeClass

#### [module monitor.Router](#apidoc.module.monitor.Router)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Router ()](#apidoc.element.monitor.Router.Router)
1.  [function <span class="apidocSignatureSpan">monitor.Router.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Router.extend)
1.  object <span class="apidocSignatureSpan">monitor.Router.</span>__super__

#### [module monitor.Router.prototype](#apidoc.module.monitor.Router.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>addConnection (options)](#apidoc.element.monitor.Router.prototype.addConnection)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>addHostConnections (hostName, callback)](#apidoc.element.monitor.Router.prototype.addHostConnections)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>buildProbeKey (probeJSON)](#apidoc.element.monitor.Router.prototype.buildProbeKey)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>connectExternal (monitorJSON, connection, callback)](#apidoc.element.monitor.Router.prototype.connectExternal)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>connectInternal (monitorJSON, callback)](#apidoc.element.monitor.Router.prototype.connectInternal)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>connectMonitor (monitor, callback)](#apidoc.element.monitor.Router.prototype.connectMonitor)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>constructor ()](#apidoc.element.monitor.Router.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>determineConnection (monitorJSON, makeNewConnections, callback)](#apidoc.element.monitor.Router.prototype.determineConnection)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>disconnectExternal (connection, probeId, callback)](#apidoc.element.monitor.Router.prototype.disconnectExternal)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>disconnectInternal (probeId, callback)](#apidoc.element.monitor.Router.prototype.disconnectInternal)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>disconnectMonitor (monitor, reason, callback)](#apidoc.element.monitor.Router.prototype.disconnectMonitor)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>findConnection (hostName, appName, appInstance)](#apidoc.element.monitor.Router.prototype.findConnection)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>findConnections (hostName, appName)](#apidoc.element.monitor.Router.prototype.findConnections)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>getHostName ()](#apidoc.element.monitor.Router.prototype.getHostName)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>initialize ()](#apidoc.element.monitor.Router.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>removeConnection (connection)](#apidoc.element.monitor.Router.prototype.removeConnection)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>setFirewall (firewall)](#apidoc.element.monitor.Router.prototype.setFirewall)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>setGateway (options)](#apidoc.element.monitor.Router.prototype.setGateway)
1.  [function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>setHostName (name)](#apidoc.element.monitor.Router.prototype.setHostName)

#### [module monitor.Server](#apidoc.module.monitor.Server)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Server ()](#apidoc.element.monitor.Server.Server)
1.  [function <span class="apidocSignatureSpan">monitor.Server.</span>List ()](#apidoc.element.monitor.Server.List)
1.  [function <span class="apidocSignatureSpan">monitor.Server.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Server.extend)
1.  object <span class="apidocSignatureSpan">monitor.Server.</span>__super__

#### [module monitor.Server.List](#apidoc.module.monitor.Server.List)
1.  [function <span class="apidocSignatureSpan">monitor.Server.</span>List ()](#apidoc.element.monitor.Server.List.List)
1.  [function <span class="apidocSignatureSpan">monitor.Server.List.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Server.List.extend)
1.  object <span class="apidocSignatureSpan">monitor.Server.List.</span>__super__

#### [module monitor.Server.List.prototype](#apidoc.module.monitor.Server.List.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Server.List.prototype.</span>constructor ()](#apidoc.element.monitor.Server.List.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.Server.List.prototype.</span>model ()](#apidoc.element.monitor.Server.List.prototype.model)

#### [module monitor.Server.prototype](#apidoc.module.monitor.Server.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>bindEvents (callback)](#apidoc.element.monitor.Server.prototype.bindEvents)
1.  [function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>constructor ()](#apidoc.element.monitor.Server.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>initialize (params)](#apidoc.element.monitor.Server.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>start (options, callback)](#apidoc.element.monitor.Server.prototype.start)
1.  [function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>stop (callback)](#apidoc.element.monitor.Server.prototype.stop)

#### [module monitor.Stat](#apidoc.module.monitor.Stat)
1.  [function <span class="apidocSignatureSpan">monitor.</span>Stat (module)](#apidoc.element.monitor.Stat.Stat)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>_buildRegex (str)](#apidoc.element.monitor.Stat._buildRegex)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>_emit (module, name, value, type)](#apidoc.element.monitor.Stat._emit)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>addListener (type, listener)](#apidoc.element.monitor.Stat.addListener)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>emit (type)](#apidoc.element.monitor.Stat.emit)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>eventNames ()](#apidoc.element.monitor.Stat.eventNames)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>getMaxListeners ()](#apidoc.element.monitor.Stat.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>listenerCount (type)](#apidoc.element.monitor.Stat.listenerCount)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>listeners (type)](#apidoc.element.monitor.Stat.listeners)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>on (type, listener)](#apidoc.element.monitor.Stat.on)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>once (type, listener)](#apidoc.element.monitor.Stat.once)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>prependListener (type, listener)](#apidoc.element.monitor.Stat.prependListener)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>prependOnceListener (type, listener)](#apidoc.element.monitor.Stat.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>removeAllListeners (type)](#apidoc.element.monitor.Stat.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>removeListener (type, listener)](#apidoc.element.monitor.Stat.removeListener)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.</span>setMaxListeners (n)](#apidoc.element.monitor.Stat.setMaxListeners)
1.  object <span class="apidocSignatureSpan">monitor.Stat.</span>eventRegex
1.  undefined <span class="apidocSignatureSpan">monitor.Stat.</span>domain

#### [module monitor.Stat.prototype](#apidoc.module.monitor.Stat.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.prototype.</span>decrement (name, value)](#apidoc.element.monitor.Stat.prototype.decrement)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.prototype.</span>gauge (name, value)](#apidoc.element.monitor.Stat.prototype.gauge)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.prototype.</span>increment (name, value)](#apidoc.element.monitor.Stat.prototype.increment)
1.  [function <span class="apidocSignatureSpan">monitor.Stat.prototype.</span>time (name, duration)](#apidoc.element.monitor.Stat.prototype.time)

#### [module monitor.StatProbe](#apidoc.module.monitor.StatProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>StatProbe ()](#apidoc.element.monitor.StatProbe.StatProbe)
1.  [function <span class="apidocSignatureSpan">monitor.StatProbe.</span>List ()](#apidoc.element.monitor.StatProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.StatProbe.</span>extend (params)](#apidoc.element.monitor.StatProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.StatProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.StatProbe.</span>classes

#### [module monitor.StatProbe.prototype](#apidoc.module.monitor.StatProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.StatProbe.prototype.</span>constructor ()](#apidoc.element.monitor.StatProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.StatProbe.prototype.</span>initialize ()](#apidoc.element.monitor.StatProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.StatProbe.prototype.</span>release ()](#apidoc.element.monitor.StatProbe.prototype.release)
1.  object <span class="apidocSignatureSpan">monitor.StatProbe.prototype.</span>defaults
1.  string <span class="apidocSignatureSpan">monitor.StatProbe.prototype.</span>probeClass

#### [module monitor.StreamProbe](#apidoc.module.monitor.StreamProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>StreamProbe ()](#apidoc.element.monitor.StreamProbe.StreamProbe)
1.  [function <span class="apidocSignatureSpan">monitor.StreamProbe.</span>List ()](#apidoc.element.monitor.StreamProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.StreamProbe.</span>extend (params)](#apidoc.element.monitor.StreamProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.StreamProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.StreamProbe.</span>classes

#### [module monitor.StreamProbe.prototype](#apidoc.module.monitor.StreamProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.StreamProbe.prototype.</span>_send ()](#apidoc.element.monitor.StreamProbe.prototype._send)
1.  [function <span class="apidocSignatureSpan">monitor.StreamProbe.prototype.</span>constructor ()](#apidoc.element.monitor.StreamProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.StreamProbe.prototype.</span>initialize ()](#apidoc.element.monitor.StreamProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.StreamProbe.prototype.</span>queueItem (item)](#apidoc.element.monitor.StreamProbe.prototype.queueItem)
1.  object <span class="apidocSignatureSpan">monitor.StreamProbe.prototype.</span>defaults

#### [module monitor.SyncProbe](#apidoc.module.monitor.SyncProbe)
1.  [function <span class="apidocSignatureSpan">monitor.</span>SyncProbe ()](#apidoc.element.monitor.SyncProbe.SyncProbe)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.</span>FileSyncProbe ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.</span>List ()](#apidoc.element.monitor.SyncProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.</span>extend (params)](#apidoc.element.monitor.SyncProbe.extend)
1.  object <span class="apidocSignatureSpan">monitor.SyncProbe.</span>Config
1.  object <span class="apidocSignatureSpan">monitor.SyncProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.SyncProbe.</span>classes

#### [module monitor.SyncProbe.FileSyncProbe](#apidoc.module.monitor.SyncProbe.FileSyncProbe)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.</span>FileSyncProbe ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.FileSyncProbe)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>List ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.List)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>extend (params)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.extend)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>getRootPath ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.getRootPath)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>setRootPath (rootPath)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.setRootPath)
1.  object <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>__super__
1.  object <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>classes

#### [module monitor.SyncProbe.FileSyncProbe.prototype](#apidoc.module.monitor.SyncProbe.FileSyncProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>constructor ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>create_control (args, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.create_control)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>delete_control (args, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.delete_control)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>getFullPath (modelId, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.getFullPath)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>read_control (args, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.read_control)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>release ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.release)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>update_control (args, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.update_control)
1.  string <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>probeClass

#### [module monitor.SyncProbe.prototype](#apidoc.module.monitor.SyncProbe.prototype)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>constructor ()](#apidoc.element.monitor.SyncProbe.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>create_control (args, callback)](#apidoc.element.monitor.SyncProbe.prototype.create_control)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>delete_control (args, callback)](#apidoc.element.monitor.SyncProbe.prototype.delete_control)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.SyncProbe.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>read_control (args, callback)](#apidoc.element.monitor.SyncProbe.prototype.read_control)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>release ()](#apidoc.element.monitor.SyncProbe.prototype.release)
1.  [function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>update_control (args, callback)](#apidoc.element.monitor.SyncProbe.prototype.update_control)
1.  object <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>defaults
1.  string <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>probeClass

#### [module monitor._](#apidoc.module.monitor._)
1.  [function <span class="apidocSignatureSpan">monitor.</span>_ (obj)](#apidoc.element.monitor._._)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>after (times, func)](#apidoc.element.monitor._.after)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>all (obj, iterator, context)](#apidoc.element.monitor._.all)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>any (obj, iterator, context)](#apidoc.element.monitor._.any)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>bind (func, context)](#apidoc.element.monitor._.bind)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>bindAll (obj)](#apidoc.element.monitor._.bindAll)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>chain (obj)](#apidoc.element.monitor._.chain)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>clone (obj)](#apidoc.element.monitor._.clone)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>collect (obj, iterator, context)](#apidoc.element.monitor._.collect)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>compact (array)](#apidoc.element.monitor._.compact)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>compose ()](#apidoc.element.monitor._.compose)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>contains (obj, target)](#apidoc.element.monitor._.contains)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>countBy (obj, value, context)](#apidoc.element.monitor._.countBy)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>debounce (func, wait, immediate)](#apidoc.element.monitor._.debounce)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>defaults (obj)](#apidoc.element.monitor._.defaults)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>defer (func)](#apidoc.element.monitor._.defer)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>delay (func, wait)](#apidoc.element.monitor._.delay)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>detect (obj, iterator, context)](#apidoc.element.monitor._.detect)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>difference (array)](#apidoc.element.monitor._.difference)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>drop (array, n, guard)](#apidoc.element.monitor._.drop)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>each (obj, iterator, context)](#apidoc.element.monitor._.each)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>escape (string)](#apidoc.element.monitor._.escape)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>every (obj, iterator, context)](#apidoc.element.monitor._.every)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>extend (obj)](#apidoc.element.monitor._.extend)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>filter (obj, iterator, context)](#apidoc.element.monitor._.filter)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>find (obj, iterator, context)](#apidoc.element.monitor._.find)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>findWhere (obj, attrs)](#apidoc.element.monitor._.findWhere)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>first (array, n, guard)](#apidoc.element.monitor._.first)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>flatten (array, shallow)](#apidoc.element.monitor._.flatten)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>foldl (obj, iterator, memo, context)](#apidoc.element.monitor._.foldl)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>foldr (obj, iterator, memo, context)](#apidoc.element.monitor._.foldr)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>forEach (obj, iterator, context)](#apidoc.element.monitor._.forEach)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>functions (obj)](#apidoc.element.monitor._.functions)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>groupBy (obj, value, context)](#apidoc.element.monitor._.groupBy)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>has (obj, key)](#apidoc.element.monitor._.has)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>head (array, n, guard)](#apidoc.element.monitor._.head)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>identity (value)](#apidoc.element.monitor._.identity)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>include (obj, target)](#apidoc.element.monitor._.include)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>indexOf (array, item, isSorted)](#apidoc.element.monitor._.indexOf)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>initial (array, n, guard)](#apidoc.element.monitor._.initial)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>inject (obj, iterator, memo, context)](#apidoc.element.monitor._.inject)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>intersection (array)](#apidoc.element.monitor._.intersection)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>invert (obj)](#apidoc.element.monitor._.invert)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>invoke (obj, method)](#apidoc.element.monitor._.invoke)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isArguments (obj)](#apidoc.element.monitor._.isArguments)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isArray ()](#apidoc.element.monitor._.isArray)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isBoolean (obj)](#apidoc.element.monitor._.isBoolean)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isDate (obj)](#apidoc.element.monitor._.isDate)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isElement (obj)](#apidoc.element.monitor._.isElement)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isEmpty (obj)](#apidoc.element.monitor._.isEmpty)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isEqual (a, b)](#apidoc.element.monitor._.isEqual)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isFinite (obj)](#apidoc.element.monitor._.isFinite)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isFunction (obj)](#apidoc.element.monitor._.isFunction)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isNaN (obj)](#apidoc.element.monitor._.isNaN)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isNull (obj)](#apidoc.element.monitor._.isNull)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isNumber (obj)](#apidoc.element.monitor._.isNumber)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isObject (obj)](#apidoc.element.monitor._.isObject)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isRegExp (obj)](#apidoc.element.monitor._.isRegExp)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isString (obj)](#apidoc.element.monitor._.isString)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>isUndefined (obj)](#apidoc.element.monitor._.isUndefined)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>keys ()](#apidoc.element.monitor._.keys)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>last (array, n, guard)](#apidoc.element.monitor._.last)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>lastIndexOf (array, item, from)](#apidoc.element.monitor._.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>map (obj, iterator, context)](#apidoc.element.monitor._.map)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>max (obj, iterator, context)](#apidoc.element.monitor._.max)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>memoize (func, hasher)](#apidoc.element.monitor._.memoize)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>methods (obj)](#apidoc.element.monitor._.methods)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>min (obj, iterator, context)](#apidoc.element.monitor._.min)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>mixin (obj)](#apidoc.element.monitor._.mixin)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>noConflict ()](#apidoc.element.monitor._.noConflict)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>object (list, values)](#apidoc.element.monitor._.object)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>omit (obj)](#apidoc.element.monitor._.omit)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>once (func)](#apidoc.element.monitor._.once)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>pairs (obj)](#apidoc.element.monitor._.pairs)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>partial (func)](#apidoc.element.monitor._.partial)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>pick (obj)](#apidoc.element.monitor._.pick)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>pluck (obj, key)](#apidoc.element.monitor._.pluck)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>random (min, max)](#apidoc.element.monitor._.random)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>range (start, stop, step)](#apidoc.element.monitor._.range)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>reduce (obj, iterator, memo, context)](#apidoc.element.monitor._.reduce)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>reduceRight (obj, iterator, memo, context)](#apidoc.element.monitor._.reduceRight)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>reject (obj, iterator, context)](#apidoc.element.monitor._.reject)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>rest (array, n, guard)](#apidoc.element.monitor._.rest)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>result (object, property)](#apidoc.element.monitor._.result)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>select (obj, iterator, context)](#apidoc.element.monitor._.select)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>shuffle (obj)](#apidoc.element.monitor._.shuffle)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>size (obj)](#apidoc.element.monitor._.size)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>some (obj, iterator, context)](#apidoc.element.monitor._.some)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>sortBy (obj, value, context)](#apidoc.element.monitor._.sortBy)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>sortedIndex (array, obj, iterator, context)](#apidoc.element.monitor._.sortedIndex)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>tail (array, n, guard)](#apidoc.element.monitor._.tail)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>take (array, n, guard)](#apidoc.element.monitor._.take)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>tap (obj, interceptor)](#apidoc.element.monitor._.tap)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>template (text, data, settings)](#apidoc.element.monitor._.template)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>throttle (func, wait)](#apidoc.element.monitor._.throttle)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>times (n, iterator, context)](#apidoc.element.monitor._.times)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>toArray (obj)](#apidoc.element.monitor._.toArray)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>unescape (string)](#apidoc.element.monitor._.unescape)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>union ()](#apidoc.element.monitor._.union)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>uniq (array, isSorted, iterator, context)](#apidoc.element.monitor._.uniq)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>unique (array, isSorted, iterator, context)](#apidoc.element.monitor._.unique)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>uniqueId (prefix)](#apidoc.element.monitor._.uniqueId)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>values (obj)](#apidoc.element.monitor._.values)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>where (obj, attrs, first)](#apidoc.element.monitor._.where)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>without (array)](#apidoc.element.monitor._.without)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>wrap (func, wrapper)](#apidoc.element.monitor._.wrap)
1.  [function <span class="apidocSignatureSpan">monitor._.</span>zip ()](#apidoc.element.monitor._.zip)
1.  object <span class="apidocSignatureSpan">monitor._.</span>templateSettings
1.  string <span class="apidocSignatureSpan">monitor._.</span>VERSION

#### [module monitor._.prototype](#apidoc.module.monitor._.prototype)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>_ ()](#apidoc.element.monitor._.prototype._)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>after ()](#apidoc.element.monitor._.prototype.after)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>all ()](#apidoc.element.monitor._.prototype.all)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>any ()](#apidoc.element.monitor._.prototype.any)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>bind ()](#apidoc.element.monitor._.prototype.bind)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>bindAll ()](#apidoc.element.monitor._.prototype.bindAll)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>chain ()](#apidoc.element.monitor._.prototype.chain)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>clone ()](#apidoc.element.monitor._.prototype.clone)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>collect ()](#apidoc.element.monitor._.prototype.collect)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>compact ()](#apidoc.element.monitor._.prototype.compact)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>compose ()](#apidoc.element.monitor._.prototype.compose)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>concat ()](#apidoc.element.monitor._.prototype.concat)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>contains ()](#apidoc.element.monitor._.prototype.contains)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>countBy ()](#apidoc.element.monitor._.prototype.countBy)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>debounce ()](#apidoc.element.monitor._.prototype.debounce)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>defaults ()](#apidoc.element.monitor._.prototype.defaults)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>defer ()](#apidoc.element.monitor._.prototype.defer)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>delay ()](#apidoc.element.monitor._.prototype.delay)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>detect ()](#apidoc.element.monitor._.prototype.detect)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>difference ()](#apidoc.element.monitor._.prototype.difference)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>drop ()](#apidoc.element.monitor._.prototype.drop)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>each ()](#apidoc.element.monitor._.prototype.each)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>escape ()](#apidoc.element.monitor._.prototype.escape)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>every ()](#apidoc.element.monitor._.prototype.every)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>extend ()](#apidoc.element.monitor._.prototype.extend)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>filter ()](#apidoc.element.monitor._.prototype.filter)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>find ()](#apidoc.element.monitor._.prototype.find)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>findWhere ()](#apidoc.element.monitor._.prototype.findWhere)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>first ()](#apidoc.element.monitor._.prototype.first)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>flatten ()](#apidoc.element.monitor._.prototype.flatten)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>foldl ()](#apidoc.element.monitor._.prototype.foldl)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>foldr ()](#apidoc.element.monitor._.prototype.foldr)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>forEach ()](#apidoc.element.monitor._.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>functions ()](#apidoc.element.monitor._.prototype.functions)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>groupBy ()](#apidoc.element.monitor._.prototype.groupBy)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>has ()](#apidoc.element.monitor._.prototype.has)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>head ()](#apidoc.element.monitor._.prototype.head)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>identity ()](#apidoc.element.monitor._.prototype.identity)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>include ()](#apidoc.element.monitor._.prototype.include)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>indexOf ()](#apidoc.element.monitor._.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>initial ()](#apidoc.element.monitor._.prototype.initial)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>inject ()](#apidoc.element.monitor._.prototype.inject)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>intersection ()](#apidoc.element.monitor._.prototype.intersection)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>invert ()](#apidoc.element.monitor._.prototype.invert)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>invoke ()](#apidoc.element.monitor._.prototype.invoke)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isArguments ()](#apidoc.element.monitor._.prototype.isArguments)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isArray ()](#apidoc.element.monitor._.prototype.isArray)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isBoolean ()](#apidoc.element.monitor._.prototype.isBoolean)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isDate ()](#apidoc.element.monitor._.prototype.isDate)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isElement ()](#apidoc.element.monitor._.prototype.isElement)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isEmpty ()](#apidoc.element.monitor._.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isEqual ()](#apidoc.element.monitor._.prototype.isEqual)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isFinite ()](#apidoc.element.monitor._.prototype.isFinite)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isFunction ()](#apidoc.element.monitor._.prototype.isFunction)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isNaN ()](#apidoc.element.monitor._.prototype.isNaN)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isNull ()](#apidoc.element.monitor._.prototype.isNull)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isNumber ()](#apidoc.element.monitor._.prototype.isNumber)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isObject ()](#apidoc.element.monitor._.prototype.isObject)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isRegExp ()](#apidoc.element.monitor._.prototype.isRegExp)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isString ()](#apidoc.element.monitor._.prototype.isString)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>isUndefined ()](#apidoc.element.monitor._.prototype.isUndefined)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>join ()](#apidoc.element.monitor._.prototype.join)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>keys ()](#apidoc.element.monitor._.prototype.keys)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>last ()](#apidoc.element.monitor._.prototype.last)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>lastIndexOf ()](#apidoc.element.monitor._.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>map ()](#apidoc.element.monitor._.prototype.map)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>max ()](#apidoc.element.monitor._.prototype.max)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>memoize ()](#apidoc.element.monitor._.prototype.memoize)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>methods ()](#apidoc.element.monitor._.prototype.methods)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>min ()](#apidoc.element.monitor._.prototype.min)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>mixin ()](#apidoc.element.monitor._.prototype.mixin)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>noConflict ()](#apidoc.element.monitor._.prototype.noConflict)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>object ()](#apidoc.element.monitor._.prototype.object)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>omit ()](#apidoc.element.monitor._.prototype.omit)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>once ()](#apidoc.element.monitor._.prototype.once)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>pairs ()](#apidoc.element.monitor._.prototype.pairs)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>partial ()](#apidoc.element.monitor._.prototype.partial)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>pick ()](#apidoc.element.monitor._.prototype.pick)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>pluck ()](#apidoc.element.monitor._.prototype.pluck)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>pop ()](#apidoc.element.monitor._.prototype.pop)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>push ()](#apidoc.element.monitor._.prototype.push)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>random ()](#apidoc.element.monitor._.prototype.random)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>range ()](#apidoc.element.monitor._.prototype.range)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>reduce ()](#apidoc.element.monitor._.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>reduceRight ()](#apidoc.element.monitor._.prototype.reduceRight)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>reject ()](#apidoc.element.monitor._.prototype.reject)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>rest ()](#apidoc.element.monitor._.prototype.rest)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>result ()](#apidoc.element.monitor._.prototype.result)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>reverse ()](#apidoc.element.monitor._.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>select ()](#apidoc.element.monitor._.prototype.select)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>shift ()](#apidoc.element.monitor._.prototype.shift)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>shuffle ()](#apidoc.element.monitor._.prototype.shuffle)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>size ()](#apidoc.element.monitor._.prototype.size)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>slice ()](#apidoc.element.monitor._.prototype.slice)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>some ()](#apidoc.element.monitor._.prototype.some)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>sort ()](#apidoc.element.monitor._.prototype.sort)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>sortBy ()](#apidoc.element.monitor._.prototype.sortBy)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>sortedIndex ()](#apidoc.element.monitor._.prototype.sortedIndex)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>splice ()](#apidoc.element.monitor._.prototype.splice)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>tail ()](#apidoc.element.monitor._.prototype.tail)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>take ()](#apidoc.element.monitor._.prototype.take)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>tap ()](#apidoc.element.monitor._.prototype.tap)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>template ()](#apidoc.element.monitor._.prototype.template)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>throttle ()](#apidoc.element.monitor._.prototype.throttle)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>times ()](#apidoc.element.monitor._.prototype.times)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>toArray ()](#apidoc.element.monitor._.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>unescape ()](#apidoc.element.monitor._.prototype.unescape)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>union ()](#apidoc.element.monitor._.prototype.union)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>uniq ()](#apidoc.element.monitor._.prototype.uniq)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>unique ()](#apidoc.element.monitor._.prototype.unique)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>uniqueId ()](#apidoc.element.monitor._.prototype.uniqueId)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>unshift ()](#apidoc.element.monitor._.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>value ()](#apidoc.element.monitor._.prototype.value)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>values ()](#apidoc.element.monitor._.prototype.values)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>where ()](#apidoc.element.monitor._.prototype.where)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>without ()](#apidoc.element.monitor._.prototype.without)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>wrap ()](#apidoc.element.monitor._.prototype.wrap)
1.  [function <span class="apidocSignatureSpan">monitor._.prototype.</span>zip ()](#apidoc.element.monitor._.prototype.zip)

#### [module monitor.__super__](#apidoc.module.monitor.__super__)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>_computeChanges (loud)](#apidoc.element.monitor.__super__._computeChanges)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>_validate (attrs, options)](#apidoc.element.monitor.__super__._validate)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>bind (name, callback, context)](#apidoc.element.monitor.__super__.bind)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>change (options)](#apidoc.element.monitor.__super__.change)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>changedAttributes (diff)](#apidoc.element.monitor.__super__.changedAttributes)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>clear (options)](#apidoc.element.monitor.__super__.clear)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>clone ()](#apidoc.element.monitor.__super__.clone)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>destroy ()](#apidoc.element.monitor.__super__.destroy)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>escape (attr)](#apidoc.element.monitor.__super__.escape)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>fetch ()](#apidoc.element.monitor.__super__.fetch)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>get (attr)](#apidoc.element.monitor.__super__.get)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>has (attr)](#apidoc.element.monitor.__super__.has)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>hasChanged (attr)](#apidoc.element.monitor.__super__.hasChanged)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>initialize ()](#apidoc.element.monitor.__super__.initialize)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>isNew ()](#apidoc.element.monitor.__super__.isNew)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>listenTo (object, events, callback)](#apidoc.element.monitor.__super__.listenTo)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>off (name, callback, context)](#apidoc.element.monitor.__super__.off)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>on (name, callback, context)](#apidoc.element.monitor.__super__.on)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>once (name, callback, context)](#apidoc.element.monitor.__super__.once)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>parse (resp)](#apidoc.element.monitor.__super__.parse)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>previous (attr)](#apidoc.element.monitor.__super__.previous)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>previousAttributes ()](#apidoc.element.monitor.__super__.previousAttributes)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>save ()](#apidoc.element.monitor.__super__.save)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>set (key, val, options)](#apidoc.element.monitor.__super__.set)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>stopListening (object, events, callback)](#apidoc.element.monitor.__super__.stopListening)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>sync ()](#apidoc.element.monitor.__super__.sync)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>toJSON (options)](#apidoc.element.monitor.__super__.toJSON)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>trigger (name)](#apidoc.element.monitor.__super__.trigger)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>unbind (name, callback, context)](#apidoc.element.monitor.__super__.unbind)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>unset (attr, options)](#apidoc.element.monitor.__super__.unset)
1.  [function <span class="apidocSignatureSpan">monitor.__super__.</span>url ()](#apidoc.element.monitor.__super__.url)
1.  object <span class="apidocSignatureSpan">monitor.__super__.</span>changed
1.  string <span class="apidocSignatureSpan">monitor.__super__.</span>idAttribute



# <a name="apidoc.module.monitor"></a>[module monitor](#apidoc.module.monitor)

#### <a name="apidoc.element.monitor.Backbone.Collection"></a>[function <span class="apidocSignatureSpan">monitor.</span>Backbone.Collection (models, options)](#apidoc.element.monitor.Backbone.Collection)
- description and source-code
```javascript
Backbone.Collection = function (models, options) {
  options || (options = {});
  if (options.model) this.model = options.model;
  if (options.comparator !== void 0) this.comparator = options.comparator;
  this._reset();
  this.initialize.apply(this, arguments);
  if (models) this.reset(models, _.extend({silent: true}, options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History"></a>[function <span class="apidocSignatureSpan">monitor.</span>Backbone.History ()](#apidoc.element.monitor.Backbone.History)
- description and source-code
```javascript
Backbone.History = function () {
  this.handlers = [];
  _.bindAll(this, 'checkUrl');

  // #1653 - Ensure that 'History' can be used outside of the browser.
  if (typeof window !== 'undefined') {
    this.location = window.location;
    this.history = window.history;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Model"></a>[function <span class="apidocSignatureSpan">monitor.</span>Backbone.Model (attributes, options)](#apidoc.element.monitor.Backbone.Model)
- description and source-code
```javascript
Backbone.Model = function (attributes, options) {
  var defaults;
  var attrs = attributes || {};
  this.cid = _.uniqueId('c');
  this.changed = {};
  this.attributes = {};
  this._changes = [];
  if (options && options.collection) this.collection = options.collection;
  if (options && options.parse) attrs = this.parse(attrs);
  if (defaults = _.result(this, 'defaults')) _.defaults(attrs, defaults);
  this.set(attrs, {silent: true});
  this._currentAttributes = _.clone(this.attributes);
  this._previousAttributes = _.clone(this.attributes);
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router"></a>[function <span class="apidocSignatureSpan">monitor.</span>Backbone.Router (options)](#apidoc.element.monitor.Backbone.Router)
- description and source-code
```javascript
Backbone.Router = function (options) {
  options || (options = {});
  if (options.routes) this.routes = options.routes;
  this._bindRoutes();
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View"></a>[function <span class="apidocSignatureSpan">monitor.</span>Backbone.View (options)](#apidoc.element.monitor.Backbone.View)
- description and source-code
```javascript
Backbone.View = function (options) {
  this.cid = _.uniqueId('view');
  this._configure(options || {});
  this._ensureElement();
  this.initialize.apply(this, arguments);
  this.delegateEvents();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Connection"></a>[function <span class="apidocSignatureSpan">monitor.</span>Connection ()](#apidoc.element.monitor.Connection)
- description and source-code
```javascript
Connection = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Connection.List"></a>[function <span class="apidocSignatureSpan">monitor.</span>Connection.List ()](#apidoc.element.monitor.Connection.List)
- description and source-code
```javascript
Connection.List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Cron.CronJob"></a>[function <span class="apidocSignatureSpan">monitor.</span>Cron.CronJob (cronTime, event, oncomplete)](#apidoc.element.monitor.Cron.CronJob)
- description and source-code
```javascript
function CronJob(cronTime, event, oncomplete) {

  if (!(this instanceof CronJob)) {
    return new CronJob(cronTime, event);
  }

  this.events = [event];
  this.cronTime = new CronTime(cronTime);
  this.now = {};
  this.initiated = false;
  this.oncomplete = oncomplete;

  this.clock();

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Cron.CronTime"></a>[function <span class="apidocSignatureSpan">monitor.</span>Cron.CronTime (time)](#apidoc.element.monitor.Cron.CronTime)
- description and source-code
```javascript
function CronTime(time) {

  this.source = time;

  this.map = ['second', 'minute', 'hour', 'dayOfMonth', 'month', 'dayOfWeek'];
  this.constraints = [[0,59],[0,59],[0,23],[1,31],[0,11],[1,7]];
  this.aliases = {
    jan:0,feb:1,mar:2,apr:3,may:4,jun:5,jul:6,aug:7,sep:8,oct:9,nov:10,dec:11,
    sun:1,mon:2,tue:3,wed:4,thu:5,fri:6,sat:7
  };

  this.second = {};
  this.minute = {};
  this.hour = {};
  this.dayOfMonth = {};
  this.month = {};
  this.dayOfWeek = {};

  this._parse();

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>DataModelProbe ()](#apidoc.element.monitor.DataModelProbe)
- description and source-code
```javascript
DataModelProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.</span>DataModelProbe.List ()](#apidoc.element.monitor.DataModelProbe.List)
- description and source-code
```javascript
DataModelProbe.List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>FileProbe ()](#apidoc.element.monitor.FileProbe)
- description and source-code
```javascript
FileProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.InspectProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>InspectProbe ()](#apidoc.element.monitor.InspectProbe)
- description and source-code
```javascript
InspectProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.List"></a>[function <span class="apidocSignatureSpan">monitor.</span>List ()](#apidoc.element.monitor.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.Log"></a>[function <span class="apidocSignatureSpan">monitor.</span>Log (module)](#apidoc.element.monitor.Log)
- description and source-code
```javascript
Log = function (module) {
  var t = this;
  t.module = module;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.LogProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>LogProbe ()](#apidoc.element.monitor.LogProbe)
- description and source-code
```javascript
LogProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.PollingProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>PollingProbe ()](#apidoc.element.monitor.PollingProbe)
- description and source-code
```javascript
PollingProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Probe"></a>[function <span class="apidocSignatureSpan">monitor.</span>Probe ()](#apidoc.element.monitor.Probe)
- description and source-code
```javascript
Probe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ProcessProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>ProcessProbe ()](#apidoc.element.monitor.ProcessProbe)
- description and source-code
```javascript
ProcessProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>RecipeProbe ()](#apidoc.element.monitor.RecipeProbe)
- description and source-code
```javascript
RecipeProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ReplProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>ReplProbe ()](#apidoc.element.monitor.ReplProbe)
- description and source-code
```javascript
ReplProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Router"></a>[function <span class="apidocSignatureSpan">monitor.</span>Router ()](#apidoc.element.monitor.Router)
- description and source-code
```javascript
Router = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Server"></a>[function <span class="apidocSignatureSpan">monitor.</span>Server ()](#apidoc.element.monitor.Server)
- description and source-code
```javascript
Server = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
* due to a firewall or browser restriction, the monitor will attempt the
* connection to the probe through the gateway server.
*
* The server specified in this method must have been started as a gateway
* like this:
*
*     // Start a monitor server and act as a gateway
*     var server = new Monitor.Server({gateway:true});
*
* @method setGateway
* @param options {Object} - Connection parameters
*   @param options.hostName {String} - Name of the gateway host
*   @param options.hostPort {Integer} - Port number to connect with
*   @param options.url {String} - The URL used to connect (created, or used if supplied)
*   @param options.socket {io.socket} - Pre-connected socket.io socket to the gateway server.
...
```

#### <a name="apidoc.element.monitor.Server.List"></a>[function <span class="apidocSignatureSpan">monitor.</span>Server.List ()](#apidoc.element.monitor.Server.List)
- description and source-code
```javascript
Server.List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat"></a>[function <span class="apidocSignatureSpan">monitor.</span>Stat (module)](#apidoc.element.monitor.Stat)
- description and source-code
```javascript
Stat = function (module) {
  var t = this;
  t.module = module;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.StatProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>StatProbe ()](#apidoc.element.monitor.StatProbe)
- description and source-code
```javascript
StatProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.StreamProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>StreamProbe ()](#apidoc.element.monitor.StreamProbe)
- description and source-code
```javascript
StreamProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Sync"></a>[function <span class="apidocSignatureSpan">monitor.</span>Sync (className, options)](#apidoc.element.monitor.Sync)
- description and source-code
```javascript
Sync = function (className, options) {
  if (!className) {
    throw new Error('Sync class name must be provided');
  }

  // Get a Sync object and bind it to the sync function
  var syncObj = new Sync(className, options);
  return function(method, model, options) {
    logger.info('sync', {className: className, method:method, model:model.toJSON(), options:options});
    return syncObj._sync(method, model, options);
  };
}
```
- example usage
```shell
...
* functionality to any Backbone data model.
*
* The returned function can be assigned to the '''sync''' element when defining the
* data model:
*
*     var BlogEntry = Backbone.Model.extend({
*       ...
*       sync: Monitor.Sync('BlogEntry'),
*       ...
*     });
*
* The sync function can also be assigned to any Backbone model after construction:
*
*     var myBook = new Book({id:"44329"});
*     myBook.sync = Monitor.Sync('Book');
...
```

#### <a name="apidoc.element.monitor.SyncProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>SyncProbe ()](#apidoc.element.monitor.SyncProbe)
- description and source-code
```javascript
SyncProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>SyncProbe.FileSyncProbe ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe)
- description and source-code
```javascript
SyncProbe.FileSyncProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._"></a>[function <span class="apidocSignatureSpan">monitor.</span>_ (obj)](#apidoc.element.monitor._)
- description and source-code
```javascript
_ = function (obj) {
  if (obj instanceof _) return obj;
  if (!(this instanceof _)) return new _(obj);
  this._wrapped = obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.deepCopy"></a>[function <span class="apidocSignatureSpan">monitor.</span>deepCopy (value, depth)](#apidoc.element.monitor.deepCopy)
- description and source-code
```javascript
deepCopy = function (value, depth) {

  // Defaults
  depth = typeof(depth) === 'undefined' ? DEFAULT_DEEP_COPY_DEPTH : depth;

  // Simple value - return the raw value
  if (typeof value !== 'object' && typeof value !== 'function') {
    return value;
  }

  // Build a string representation of the type
  var strType = '[Object]';
  if (typeof value === 'function') {
    strType = '[Function]';
  } else if (Array.isArray(value)) {
    strType = '[Array]';
  }

  // Limit reached
  if (depth <= 0) {
    return strType;
  }

  // Create a new object to copy into.
  // Proactively add constructor so it's at the top of a function
  var copy = Array.isArray(value) ? [] : {};

  // Copy all elements (by reference)
  for (var prop in value) {
    if (!value.hasOwnProperty || value.hasOwnProperty(prop)) {
      var elem = value[prop];
      if (typeof elem === 'object' || typeof elem === 'function') {
        copy[prop] = Monitor.deepCopy(elem, depth - 1);
      }
      else {
        copy[prop] = elem;
      }
    }
  }

  // Special string formatting for functions
  if (typeof value === 'function') {
    if (_.isEmpty(copy)) {
      // No sub-elements.  Identify it as a function.
      copy = strType;
    } else {
      // Sub-elements exist.  Identify it as a function by placing
      // a constructor at the top of the object
      copy = _.extend({constructor: strType},copy);
    }
  }

  // Return the copy
  return copy;
}
```
- example usage
```shell
...
* @protected
* @param name {String} The message name to send
* @param args... {Mixed} Variable number of arguments to send with the message
* @param callback {Function} Called when remote sends a reply
*/
emit: function() {
  var t = this, socket = t.get('socket');
  log.info(t.logId + 'emit', Monitor.deepCopy(arguments, 5));
  socket.emit.apply(socket, arguments);
},

/**
* Bind the specified handler to the remote socket message.
*
* Only a single handler (per message name) can be bound using this method.
...
```

#### <a name="apidoc.element.monitor.extend"></a>[function <span class="apidocSignatureSpan">monitor.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```

#### <a name="apidoc.element.monitor.generateUniqueCollectionId"></a>[function <span class="apidocSignatureSpan">monitor.</span>generateUniqueCollectionId (collection, prefix)](#apidoc.element.monitor.generateUniqueCollectionId)
- description and source-code
```javascript
generateUniqueCollectionId = function (collection, prefix) {
  var id = '';
  prefix = prefix || '';

  // First time - get the largest idSequence in the collection
  if (!collection.idSequence) {
    collection.idSequence = 0;
    collection.forEach(function(item){
      var id = item.get('id') || '',
          sequence = +id.substr(prefix.length);
      if (collection.idSequence <= sequence) {
        collection.idSequence = sequence + 1;
      }
    });
  }

  return prefix + collection.idSequence++;
}
```
- example usage
```shell
...

// Default the firewall value
if (_.isUndefined(options.firewall)) {
  options = _.extend({},options, {firewall: t.firewall});
}

// Generate a unique ID for the connection
options.id = Monitor.generateUniqueCollectionId(t.connections);

var connStr = 'Conn_' + options.id;
if (options.hostName) {
  connStr += ' - ' + options.hostName + ':' + options.hostPort;
}
log.info('addConnection', connStr);
...
```

#### <a name="apidoc.element.monitor.generateUniqueId"></a>[function <span class="apidocSignatureSpan">monitor.</span>generateUniqueId ()](#apidoc.element.monitor.generateUniqueId)
- description and source-code
```javascript
generateUniqueId = function () {
  // Generate a 4 digit random hex string
  stat.increment('generateUniqueId');
  function rhs4() {return (((1 + Math.random()) * 0x10000) | 0).toString(16).substring(1);}
  return (rhs4()+rhs4()+"-"+rhs4()+"-"+rhs4()+"-"+rhs4()+"-"+rhs4()+rhs4()+rhs4());
}
```
- example usage
```shell
...
* @protected
* @return hostName {String} - The platform's host name, or an otherwise stable ID
*/
getHostName: function() {
  var localStorage = root.localStorage;
  if (!hostName) {
    if (localStorage) {hostName = localStorage.hostName;}
    hostName = hostName || Monitor.generateUniqueId();
    if (localStorage) {localStorage.hostName = hostName;}
  }
  return hostName;
},

/**
* Set the current host name.
...
```

#### <a name="apidoc.element.monitor.getLogger"></a>[function <span class="apidocSignatureSpan">monitor.</span>getLogger (module)](#apidoc.element.monitor.getLogger)
- description and source-code
```javascript
getLogger = function (module) {
  return new LoggerClass(module);
}
```
- example usage
```shell
...
// For further details and documentation:
// http://lorenwest.github.com/node-monitor
(function(root){

// Module loading
var Monitor = root.Monitor || require('./Monitor'),
    Cron = Monitor.Cron, _ = Monitor._, Backbone = Monitor.Backbone,
    log = Monitor.getLogger('Connection'),
    stat = Monitor.getStatLogger('Connection'),
    Config = Monitor.Config, SocketIO = root.io || require('socket.io-client'),
    Probe = Monitor.Probe,
    nextConnectionNum = 1;

/**
* Core monitor classes
...
```

#### <a name="apidoc.element.monitor.getRouter"></a>[function <span class="apidocSignatureSpan">monitor.</span>getRouter ()](#apidoc.element.monitor.getRouter)
- description and source-code
```javascript
getRouter = function () {

  // Instantiate a router if no default
  if (!Monitor.defaultRouter) {
    Monitor.defaultRouter = new Monitor.Router();

    // If there's a global socket.io server available,
    // then we're running on the browser.  Set the default
    // gateway to the global io socket.
    if (root.io) {
      Monitor.defaultRouter.setGateway({
        socket:root.io.connect()
      });
    }
  }

  // Return the router
  return Monitor.defaultRouter;
}
```
- example usage
```shell
...
var pid = typeof process === 'undefined' ? 1 : process.pid;

// Determine the app instance
var appInstance = '' + (typeof process === 'undefined' ? pid : process.env.NODE_APP_INSTANCE || pid);

// Exchange connection information
socket.emit('connection:info', {
  hostName:Monitor.getRouter().getHostName(),
  appName:Config.Monitor.appName,
  appInstance: appInstance,
  pid: pid,
  probeClasses: _.keys(Probe.classes),
  gateway:t.get('gateway'),
  firewall:t.get('firewall')
});
...
```

#### <a name="apidoc.element.monitor.getStatLogger"></a>[function <span class="apidocSignatureSpan">monitor.</span>getStatLogger (module)](#apidoc.element.monitor.getStatLogger)
- description and source-code
```javascript
getStatLogger = function (module) {
  return new StatLoggerClass(module);
}
```
- example usage
```shell
...
// http://lorenwest.github.com/node-monitor
(function(root){

// Module loading
var Monitor = root.Monitor || require('./Monitor'),
    Cron = Monitor.Cron, _ = Monitor._, Backbone = Monitor.Backbone,
    log = Monitor.getLogger('Connection'),
    stat = Monitor.getStatLogger('Connection'),
    Config = Monitor.Config, SocketIO = root.io || require('socket.io-client'),
    Probe = Monitor.Probe,
    nextConnectionNum = 1;

/**
* Core monitor classes
*
...
```

#### <a name="apidoc.element.monitor.setLoggerClass"></a>[function <span class="apidocSignatureSpan">monitor.</span>setLoggerClass (LoggerClass)](#apidoc.element.monitor.setLoggerClass)
- description and source-code
```javascript
setLoggerClass = function (LoggerClass) {

  // Build the getLogger function
  Monitor.getLogger = function(module) {
    return new LoggerClass(module);
  };

  // Get the logger for the Monitor module
  log = Monitor.getLogger('Monitor');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.setStatLoggerClass"></a>[function <span class="apidocSignatureSpan">monitor.</span>setStatLoggerClass (StatLoggerClass)](#apidoc.element.monitor.setStatLoggerClass)
- description and source-code
```javascript
setStatLoggerClass = function (StatLoggerClass) {

  // Build the getStatLogger function
  Monitor.getStatLogger = function(module) {
    return new StatLoggerClass(module);
  };

  // Get the logger for the Monitor module
  stat = Monitor.getStatLogger('Monitor');
}
```
- example usage
```shell
...
    return new RegExp(regexStr, modifier);
  };

  // Mixin event processing for the Stat class
  _.extend(Stat, EventEmitter);

  // Expose this class from the Monitor module
  Monitor.setStatLoggerClass(Stat);

}(this));
...
```

#### <a name="apidoc.element.monitor.start"></a>[function <span class="apidocSignatureSpan">monitor.</span>start (options, callback)](#apidoc.element.monitor.start)
- description and source-code
```javascript
start = function (options, callback) {
  log.info('start', options);
  callback = callback || function(){};

  // Get a default monitor
  if (!Monitor.defaultServer) {
    Monitor.defaultServer = new Monitor.Server();
    Monitor.defaultServer.start(options, callback);
  } else {
    callback();
  }
  return Monitor;
}
```
- example usage
```shell
...

Run the following from your app server directory

    $ npm install monitor

Then place the following line in your application bootstrap, and restart your server

    require('monitor').start();

Monitoring your app with a REPL console
---------------------------------------

Ad-hoc monitoring can be done from a REPL console.

Start up the REPL, and get the Monitor class.  Feel free to copy/paste these lines into your console:
...
```

#### <a name="apidoc.element.monitor.stop"></a>[function <span class="apidocSignatureSpan">monitor.</span>stop (callback)](#apidoc.element.monitor.stop)
- description and source-code
```javascript
stop = function (callback) {
  log.info('stop');
  callback = callback || function(){};
  if (Monitor.defaultServer) {
    Monitor.defaultServer.stop(callback);
    delete Monitor.defaultServer;
  } else {
    callback();
  }
}
```
- example usage
```shell
...
server.on('clientError', function(err){
  log.error('bindEvents', 'clientError detected on server', err);
  t.trigger('error', err);
});
server.on('close', function(err){
  server.hasEmittedClose = true;
  log.info('bindEvents.serverClose', 'Server has closed', err);
  t.stop();
});

// Start up the socket.io server.
var socketIoParams = {
  log: false
};
t.socketServer = SocketIO.listen(server, socketIoParams);
...
```

#### <a name="apidoc.element.monitor.stringify"></a>[function <span class="apidocSignatureSpan">monitor.</span>stringify (value, depth, indent)](#apidoc.element.monitor.stringify)
- description and source-code
```javascript
stringify = function (value, depth, indent) {

  // Defaults
  indent = typeof(indent) === 'undefined' ? 2 : indent;

  // Return a stringified depth-limited deep copy
  return JSON.stringify(Monitor.deepCopy(value, depth), null, indent);
}
```
- example usage
```shell
...
      };

      // Client-side listener - for persisting changes to the server
      var modelListener = function(changedModel, options) {
options = options || {};

// Don't persist unless the model is different
if (_.isEqual(JSON.parse(JSON.stringify(model)), JSON.parse(JSON.stringify(model.syncMonitor.get('model'))))) {
  logger.info('modelListener.noChanges', t.className, model.toJSON());
  return;
}

// Disconnect listeners if the ID changes
if (model.get('id') !== modelId) {
  logger.info('modelListener.alteredId', t.className, model.toJSON());
...
```

#### <a name="apidoc.element.monitor.toServerString"></a>[function <span class="apidocSignatureSpan">monitor.</span>toServerString (monitorJSON)](#apidoc.element.monitor.toServerString)
- description and source-code
```javascript
toServerString = function (monitorJSON) {
  var str = monitorJSON.hostName;
  if (monitorJSON.appName) {
    str += ':' + monitorJSON.appName;
    if (monitorJSON.appInstance) {
      str += ':' + monitorJSON.appInstance;
    }
  }
  return str;
}
```
- example usage
```shell
...
callback = callback || function(){};
var t = this,
    monitorJSON = monitor.toMonitorJSON(),
    probeJSON = null,
    probeName = monitorJSON.probeName,
    probeClass = monitorJSON.probeClass,
    startTime = Date.now(),
    monitorStr = probeClass + '.' + monitor.toServerString().replace(/:/g, '.');

// Class name must be set
if (!probeClass && !probeName) {
  var errStr = 'probeName or probeClass must be set';
  log.error('connectMonitor', errStr);
  return callback(errStr);
}
...
```



# <a name="apidoc.module.monitor.Backbone"></a>[module monitor.Backbone](#apidoc.module.monitor.Backbone)

#### <a name="apidoc.element.monitor.Backbone.Collection"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>Collection (models, options)](#apidoc.element.monitor.Backbone.Collection)
- description and source-code
```javascript
Collection = function (models, options) {
  options || (options = {});
  if (options.model) this.model = options.model;
  if (options.comparator !== void 0) this.comparator = options.comparator;
  this._reset();
  this.initialize.apply(this, arguments);
  if (models) this.reset(models, _.extend({silent: true}, options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>History ()](#apidoc.element.monitor.Backbone.History)
- description and source-code
```javascript
History = function () {
  this.handlers = [];
  _.bindAll(this, 'checkUrl');

  // #1653 - Ensure that 'History' can be used outside of the browser.
  if (typeof window !== 'undefined') {
    this.location = window.location;
    this.history = window.history;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Model"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>Model (attributes, options)](#apidoc.element.monitor.Backbone.Model)
- description and source-code
```javascript
Model = function (attributes, options) {
  var defaults;
  var attrs = attributes || {};
  this.cid = _.uniqueId('c');
  this.changed = {};
  this.attributes = {};
  this._changes = [];
  if (options && options.collection) this.collection = options.collection;
  if (options && options.parse) attrs = this.parse(attrs);
  if (defaults = _.result(this, 'defaults')) _.defaults(attrs, defaults);
  this.set(attrs, {silent: true});
  this._currentAttributes = _.clone(this.attributes);
  this._previousAttributes = _.clone(this.attributes);
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>Router (options)](#apidoc.element.monitor.Backbone.Router)
- description and source-code
```javascript
Router = function (options) {
  options || (options = {});
  if (options.routes) this.routes = options.routes;
  this._bindRoutes();
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>View (options)](#apidoc.element.monitor.Backbone.View)
- description and source-code
```javascript
View = function (options) {
  this.cid = _.uniqueId('view');
  this._configure(options || {});
  this._ensureElement();
  this.initialize.apply(this, arguments);
  this.delegateEvents();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.ajax"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>ajax ()](#apidoc.element.monitor.Backbone.ajax)
- description and source-code
```javascript
ajax = function () {
  return Backbone.$.ajax.apply(Backbone.$, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.bind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
});

// Inbound probe events
t.addEvent('probe:connect', t.probeConnect.bind(t));
t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
t.addEvent('probe:control', t.probeControl.bind(t));

// Connection events
t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
t.addEvent('connection:pong', function(){t.trigger('pong');});
...
```

#### <a name="apidoc.element.monitor.Backbone.listenTo"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.listenTo)
- description and source-code
```javascript
listenTo = function (object, events, callback) {
  var listeners = this._listeners || (this._listeners = {});
  var id = object._listenerId || (object._listenerId = _.uniqueId('l'));
  listeners[id] = object;
  object.on(events, callback || this, this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.noConflict"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>noConflict ()](#apidoc.element.monitor.Backbone.noConflict)
- description and source-code
```javascript
noConflict = function () {
  root.Backbone = previousBackbone;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.off"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
...
* @method ping
* @param callback {Function(error)} Callback when response is returned
*/
ping: function(callback) {
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
...
```

#### <a name="apidoc.element.monitor.Backbone.on"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:

    > processMonitor.on('change', function() {
    ... console.log(processMonitor.get('freemem'));
    ... });

Monitoring your app with a custom script
----------------------------------------

Using Node.js as a scripting language, you can write custom monitors that do anything Node.js can do.  Here's an example that prints
 to the console when free memory falls below a threshold.
...
```

#### <a name="apidoc.element.monitor.Backbone.once"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  if (!(eventsApi(this, 'once', name, [callback, context]) && callback)) return this;
  var self = this;
  var once = _.once(function() {
    self.off(name, once);
    callback.apply(this, arguments);
  });
  once._callback = callback;
  this.on(name, once, context);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.stopListening"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.stopListening)
- description and source-code
```javascript
stopListening = function (object, events, callback) {
  var listeners = this._listeners;
  if (!listeners) return;
  if (object) {
    object.off(events, callback, this);
    if (!events && !callback) delete listeners[object._listenerId];
  } else {
    for (var id in listeners) {
      listeners[id].off(null, null, this);
    }
    this._listeners = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.sync"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>sync (method, model, options)](#apidoc.element.monitor.Backbone.sync)
- description and source-code
```javascript
sync = function (method, model, options) {
  var type = methodMap[method];

  // Default options, unless specified.
  _.defaults(options || (options = {}), {
    emulateHTTP: Backbone.emulateHTTP,
    emulateJSON: Backbone.emulateJSON
  });

  // Default JSON-request options.
  var params = {type: type, dataType: 'json'};

  // Ensure that we have a URL.
  if (!options.url) {
    params.url = _.result(model, 'url') || urlError();
  }

  // Ensure that we have the appropriate request data.
  if (options.data == null && model && (method === 'create' || method === 'update' || method === 'patch')) {
    params.contentType = 'application/json';
    params.data = JSON.stringify(options.attrs || model.toJSON(options));
  }

  // For older servers, emulate JSON by encoding the request into an HTML-form.
  if (options.emulateJSON) {
    params.contentType = 'application/x-www-form-urlencoded';
    params.data = params.data ? {model: params.data} : {};
  }

  // For older servers, emulate HTTP by mimicking the HTTP method with '_method'
  // And an 'X-HTTP-Method-Override' header.
  if (options.emulateHTTP && (type === 'PUT' || type === 'DELETE' || type === 'PATCH')) {
    params.type = 'POST';
    if (options.emulateJSON) params.data._method = type;
    var beforeSend = options.beforeSend;
    options.beforeSend = function(xhr) {
      xhr.setRequestHeader('X-HTTP-Method-Override', type);
      if (beforeSend) return beforeSend.apply(this, arguments);
    };
  }

  // Don't process data on a non-GET request.
  if (params.type !== 'GET' && !options.emulateJSON) {
    params.processData = false;
  }

  var success = options.success;
  options.success = function(resp, status, xhr) {
    if (success) success(resp, status, xhr);
    model.trigger('sync', model, resp, options);
  };

  var error = options.error;
  options.error = function(xhr, status, thrown) {
    if (error) error(model, xhr, options);
    model.trigger('error', model, xhr, options);
  };

  // Make the request, allowing the user to override any Ajax options.
  var xhr = Backbone.ajax(_.extend(params, options));
  model.trigger('request', model, xhr, options);
  return xhr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.trigger"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>trigger (name)](#apidoc.element.monitor.Backbone.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;
  var args = slice.call(arguments, 1);
  if (!eventsApi(this, 'trigger', name, args)) return this;
  var events = this._events[name];
  var allEvents = this._events.all;
  if (events) triggerEvents(this, events, args);
  if (allEvents) triggerEvents(this, allEvents, arguments);
  return this;
}
```
- example usage
```shell
...

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
},

/**
* Is this connection with the specified host?
*
...
```

#### <a name="apidoc.element.monitor.Backbone.unbind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Backbone.Collection"></a>[module monitor.Backbone.Collection](#apidoc.module.monitor.Backbone.Collection)

#### <a name="apidoc.element.monitor.Backbone.Collection.Collection"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>Collection (models, options)](#apidoc.element.monitor.Backbone.Collection.Collection)
- description and source-code
```javascript
Collection = function (models, options) {
  options || (options = {});
  if (options.model) this.model = options.model;
  if (options.comparator !== void 0) this.comparator = options.comparator;
  this._reset();
  this.initialize.apply(this, arguments);
  if (models) this.reset(models, _.extend({silent: true}, options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.extend"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.Collection.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Backbone.Collection.prototype"></a>[module monitor.Backbone.Collection.prototype](#apidoc.module.monitor.Backbone.Collection.prototype)

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype._onModelEvent"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>_onModelEvent (event, model, collection, options)](#apidoc.element.monitor.Backbone.Collection.prototype._onModelEvent)
- description and source-code
```javascript
_onModelEvent = function (event, model, collection, options) {
  if ((event === 'add' || event === 'remove') && collection !== this) return;
  if (event === 'destroy') this.remove(model, options);
  if (model && event === 'change:' + model.idAttribute) {
    delete this._byId[model.previous(model.idAttribute)];
    if (model.id != null) this._byId[model.id] = model;
  }
  this.trigger.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype._prepareModel"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>_prepareModel (attrs, options)](#apidoc.element.monitor.Backbone.Collection.prototype._prepareModel)
- description and source-code
```javascript
_prepareModel = function (attrs, options) {
  if (attrs instanceof Model) {
    if (!attrs.collection) attrs.collection = this;
    return attrs;
  }
  options || (options = {});
  options.collection = this;
  var model = new this.model(attrs, options);
  if (!model._validate(attrs, options)) return false;
  return model;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype._removeReference"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>_removeReference (model)](#apidoc.element.monitor.Backbone.Collection.prototype._removeReference)
- description and source-code
```javascript
_removeReference = function (model) {
  if (this === model.collection) delete model.collection;
  model.off('all', this._onModelEvent, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype._reset"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>_reset ()](#apidoc.element.monitor.Backbone.Collection.prototype._reset)
- description and source-code
```javascript
_reset = function () {
  this.length = 0;
  this.models = [];
  this._byId  = {};
  this._byCid = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.add"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>add (models, options)](#apidoc.element.monitor.Backbone.Collection.prototype.add)
- description and source-code
```javascript
add = function (models, options) {
  var i, args, length, model, existing, needsSort;
  var at = options && options.at;
  var sort = ((options && options.sort) == null ? true : options.sort);
  models = _.isArray(models) ? models.slice() : [models];

  // Turn bare objects into model references, and prevent invalid models
  // from being added.
  for (i = models.length - 1; i >= 0; i--) {
    if(!(model = this._prepareModel(models[i], options))) {
      this.trigger("error", this, models[i], options);
      models.splice(i, 1);
      continue;
    }
    models[i] = model;

    existing = model.id != null && this._byId[model.id];
    // If a duplicate is found, prevent it from being added and
    // optionally merge it into the existing model.
    if (existing || this._byCid[model.cid]) {
      if (options && options.merge && existing) {
        existing.set(model.attributes, options);
        needsSort = sort;
      }
      models.splice(i, 1);
      continue;
    }

    // Listen to added models' events, and index models for lookup by
    // 'id' and by 'cid'.
    model.on('all', this._onModelEvent, this);
    this._byCid[model.cid] = model;
    if (model.id != null) this._byId[model.id] = model;
  }

  // See if sorting is needed, update 'length' and splice in new models.
  if (models.length) needsSort = sort;
  this.length += models.length;
  args = [at != null ? at : this.models.length, 0];
  push.apply(args, models);
  splice.apply(this.models, args);

  // Sort the collection if appropriate.
  if (needsSort && this.comparator && at == null) this.sort({silent: true});

  if (options && options.silent) return this;

  // Trigger 'add' events.
  while (model = models.shift()) {
    model.trigger('add', model, this, options);
  }

  return this;
}
```
- example usage
```shell
...
    connection.off('disconnect', onConnect);
    log.info('disconnected', connStr, (Date.now() - startTime) + 'ms');
  };
  connection.on('connect', onConnect);
  connection.on('disconnect', onDisconnect);

  // Add to the connections
  t.connections.add(connection);
  return connection;
},

/**
* Remove a connection from the router.
*
* This is called to remove the connection and associated routes from the router.
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.all"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>all ()](#apidoc.element.monitor.Backbone.Collection.prototype.all)
- description and source-code
```javascript
all = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.any"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>any ()](#apidoc.element.monitor.Backbone.Collection.prototype.any)
- description and source-code
```javascript
any = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.at"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>at (index)](#apidoc.element.monitor.Backbone.Collection.prototype.at)
- description and source-code
```javascript
at = function (index) {
  return this.models[index];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.bind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
});

// Inbound probe events
t.addEvent('probe:connect', t.probeConnect.bind(t));
t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
t.addEvent('probe:control', t.probeControl.bind(t));

// Connection events
t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
t.addEvent('connection:pong', function(){t.trigger('pong');});
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.chain"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>chain ()](#apidoc.element.monitor.Backbone.Collection.prototype.chain)
- description and source-code
```javascript
chain = function () {
  return _(this.models).chain();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.clone"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>clone ()](#apidoc.element.monitor.Backbone.Collection.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return new this.constructor(this.models);
}
```
- example usage
```shell
...
        var onConnect = function(error, probe) {
if (error) {return callback(error);}
probeJSON = probe.toJSON();
probeJSON.probeId = probeJSON.id; delete probeJSON.id;
monitor.probe = probe;

// Keep the last known probe state for effective updating
monitor._probeValues = _.clone(probeJSON);

// Perform the initial set silently.  This assures the initial
// probe contents are available on the connect event,
// but doesn't fire a change event before connect.
monitor.set(probeJSON, {silent:true});

// Watch the probe for changes.
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.collect"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>collect ()](#apidoc.element.monitor.Backbone.Collection.prototype.collect)
- description and source-code
```javascript
collect = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.contains"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>contains ()](#apidoc.element.monitor.Backbone.Collection.prototype.contains)
- description and source-code
```javascript
contains = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.countBy"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>countBy (value, context)](#apidoc.element.monitor.Backbone.Collection.prototype.countBy)
- description and source-code
```javascript
countBy = function (value, context) {
  var iterator = _.isFunction(value) ? value : function(model) {
    return model.get(value);
  };
  return _[method](this.models, iterator, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.create"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>create (model, options)](#apidoc.element.monitor.Backbone.Collection.prototype.create)
- description and source-code
```javascript
create = function (model, options) {
  var collection = this;
  options = options ? _.clone(options) : {};
  model = this._prepareModel(model, options);
  if (!model) return false;
  if (!options.wait) collection.add(model, options);
  var success = options.success;
  options.success = function(model, resp, options) {
    if (options.wait) collection.add(model, options);
    if (success) success(model, resp, options);
  };
  model.save(null, options);
  return model;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.detect"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>detect ()](#apidoc.element.monitor.Backbone.Collection.prototype.detect)
- description and source-code
```javascript
detect = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.each"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>each ()](#apidoc.element.monitor.Backbone.Collection.prototype.each)
- description and source-code
```javascript
each = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
...
  t.addHostCallbacks[hostName].forEach(function(cb) {
    cb(error);
  });
  delete t.addHostCallbacks[hostName];
};

// Build the list of ports already connected
t.connections.each(function(connection){
  var host = connection.get('hostName').toLowerCase();
  var port = connection.get('hostPort');
  if (host === hostName && port >= portStart && port <= portEnd) {
    connectedPorts.push(port);
  }
});
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.every"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>every ()](#apidoc.element.monitor.Backbone.Collection.prototype.every)
- description and source-code
```javascript
every = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.fetch"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>fetch ()](#apidoc.element.monitor.Backbone.Collection.prototype.fetch)
- description and source-code
```javascript
fetch = function () {

  // Connect the success/error methods for callback style requests.
  // These style callbacks don't need the model or options arguments
  // because they're in the scope of the anonymous callback function.
  var args = _.toArray(arguments), callback = args[args.length - 1];
  if (typeof callback === 'function') {

    // Remove the last element (the callback)
    args.splice(-1, 1);

    // Place options if none were specified.
    if (args.length === 0) {
      args.push({});
    }

    // Place attributes if save and only options were specified
    if (args.length === 1 && methodName === 'save') {
      args.push({});
    }
    var options = args[args.length - 1];

    // Place the success and error methods
    options.success = function(model, response) {
      callback(null, response);
    };
    options.error = function(model, response) {
      // Provide the response as the error.
      callback(response, null);
    };
  }

  // Invoke the original method
  return method.apply(this, args);
}
```
- example usage
```shell
...
*       ...
*     });
*
* The sync function can also be assigned to any Backbone model after construction:
*
*     var myBook = new Book({id:"44329"});
*     myBook.sync = Monitor.Sync('Book');
*     myBook.fetch();
*
* In addition to providing the standard '''fetch''', '''save''', and '''destroy'''
* functionality, Sync offers *live data synchronization*, updating the data model
* as changes are detected on the server.
*
*     // Turn on live data synchronization
*     myBook.fetch({liveSync:true});
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.filter"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>filter ()](#apidoc.element.monitor.Backbone.Collection.prototype.filter)
- description and source-code
```javascript
filter = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
...
    * @protected
    * @param hostName {String} - Host name to search for (null = any host)
    * @param appName {String} - App name to search for (null = any app)
    * @return connections {Array of Connection} - An array of Connection objects matching the criteria
    */
    findConnections: function(hostName, appName) {
      var t = this;
      return t.connections.filter(function(conn) {

// Host or app matches if not specified or if specified and equal
var matchesHost = !hostName || conn.isThisHost(hostName);
var matchesApp = !appName || appName === conn.get('remoteAppName');
var remoteFirewall = conn.get('remoteFirewall');

// This is a match if host + app matches, and it's not firewalled
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.find"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>find ()](#apidoc.element.monitor.Backbone.Collection.prototype.find)
- description and source-code
```javascript
find = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
...
if (t.runningProbesByKey[probeName] || Probe.classes[probeClass] != null) {
  return callback(null, null);
}

// Give named auto-start probes time to start up
var autoStarts = Monitor.Config.Monitor.autoStart;
if (probeName && !probeClass && autoStarts.length) {
  var autoStart = Monitor._.find(autoStarts, function(probeDef) {
    return probeDef.probeName === probeName;
  });
  if (autoStart) {
    setTimeout(function() {
      t.determineConnection(monitorJSON, makeNewConnections, callback);
    },10);
    return;
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.first"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>first ()](#apidoc.element.monitor.Backbone.Collection.prototype.first)
- description and source-code
```javascript
first = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.foldl"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>foldl ()](#apidoc.element.monitor.Backbone.Collection.prototype.foldl)
- description and source-code
```javascript
foldl = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.foldr"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>foldr ()](#apidoc.element.monitor.Backbone.Collection.prototype.foldr)
- description and source-code
```javascript
foldr = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.forEach"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>forEach ()](#apidoc.element.monitor.Backbone.Collection.prototype.forEach)
- description and source-code
```javascript
forEach = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
...

  // Allow probes to be externally identified by name
  if (probeJSON.probeName) {
    return probeJSON.probeName;
  }

  if (initParams) {
    _.keys(initParams).sort().forEach(function(key){
      probeKey += ':' + key + '=' + initParams[key];
    });
  }
  return probeKey;
},

/**
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.get"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>get (obj)](#apidoc.element.monitor.Backbone.Collection.prototype.get)
- description and source-code
```javascript
get = function (obj) {
  if (obj == null) return void 0;
  return this._byId[obj.id != null ? obj.id : obj] || this._byCid[obj.cid || obj];
}
```
- example usage
```shell
...
For this example, we'll monitor the *Process* probe:

    > var processMonitor = new Monitor({probeClass:'Process'});
    > processMonitor.connect();

The monitor is a [Backbone.js](http://backbonejs.org/) data model so it updates in real time, and you can get all fields with toJSON
():

    > processMonitor.get('freemem');
    86368256
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.groupBy"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>groupBy (value, context)](#apidoc.element.monitor.Backbone.Collection.prototype.groupBy)
- description and source-code
```javascript
groupBy = function (value, context) {
  var iterator = _.isFunction(value) ? value : function(model) {
    return model.get(value);
  };
  return _[method](this.models, iterator, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.head"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>head ()](#apidoc.element.monitor.Backbone.Collection.prototype.head)
- description and source-code
```javascript
head = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.include"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>include ()](#apidoc.element.monitor.Backbone.Collection.prototype.include)
- description and source-code
```javascript
include = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>indexOf ()](#apidoc.element.monitor.Backbone.Collection.prototype.indexOf)
- description and source-code
```javascript
indexOf = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
...
    set_control: function(attrs, callback) {
var t = this,
    writableAttributes = t.get('writableAttributes') || [];

// Validate the attributes are writable
if (writableAttributes !== '*') {
  for (var attrName in attrs) {
    if (writableAttributes.indexOf(attrName) < 0) {
      return callback({code:'NOT_WRITABLE', msg: 'Attribute not writable: ' + attrName});
    }
  }
}

// Set the data
var error = null;
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.initial"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>initial ()](#apidoc.element.monitor.Backbone.Collection.prototype.initial)
- description and source-code
```javascript
initial = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>initialize ()](#apidoc.element.monitor.Backbone.Collection.prototype.initialize)
- description and source-code
```javascript
initialize = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.inject"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>inject ()](#apidoc.element.monitor.Backbone.Collection.prototype.inject)
- description and source-code
```javascript
inject = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.invoke"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>invoke ()](#apidoc.element.monitor.Backbone.Collection.prototype.invoke)
- description and source-code
```javascript
invoke = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>isEmpty ()](#apidoc.element.monitor.Backbone.Collection.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.last"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>last ()](#apidoc.element.monitor.Backbone.Collection.prototype.last)
- description and source-code
```javascript
last = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>lastIndexOf ()](#apidoc.element.monitor.Backbone.Collection.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.listenTo"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.Collection.prototype.listenTo)
- description and source-code
```javascript
listenTo = function (object, events, callback) {
  var listeners = this._listeners || (this._listeners = {});
  var id = object._listenerId || (object._listenerId = _.uniqueId('l'));
  listeners[id] = object;
  object.on(events, callback || this, this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.map"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>map ()](#apidoc.element.monitor.Backbone.Collection.prototype.map)
- description and source-code
```javascript
map = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.max"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>max ()](#apidoc.element.monitor.Backbone.Collection.prototype.max)
- description and source-code
```javascript
max = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.min"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>min ()](#apidoc.element.monitor.Backbone.Collection.prototype.min)
- description and source-code
```javascript
min = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.model"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>model (attributes, options)](#apidoc.element.monitor.Backbone.Collection.prototype.model)
- description and source-code
```javascript
model = function (attributes, options) {
  var defaults;
  var attrs = attributes || {};
  this.cid = _.uniqueId('c');
  this.changed = {};
  this.attributes = {};
  this._changes = [];
  if (options && options.collection) this.collection = options.collection;
  if (options && options.parse) attrs = this.parse(attrs);
  if (defaults = _.result(this, 'defaults')) _.defaults(attrs, defaults);
  this.set(attrs, {silent: true});
  this._currentAttributes = _.clone(this.attributes);
  this._previousAttributes = _.clone(this.attributes);
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.off"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
...
* @method ping
* @param callback {Function(error)} Callback when response is returned
*/
ping: function(callback) {
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.on"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:

    > processMonitor.on('change', function() {
    ... console.log(processMonitor.get('freemem'));
    ... });

Monitoring your app with a custom script
----------------------------------------

Using Node.js as a scripting language, you can write custom monitors that do anything Node.js can do.  Here's an example that prints
 to the console when free memory falls below a threshold.
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.once"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  if (!(eventsApi(this, 'once', name, [callback, context]) && callback)) return this;
  var self = this;
  var once = _.once(function() {
    self.off(name, once);
    callback.apply(this, arguments);
  });
  once._callback = callback;
  this.on(name, once, context);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.parse"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>parse (resp)](#apidoc.element.monitor.Backbone.Collection.prototype.parse)
- description and source-code
```javascript
parse = function (resp) {
  return resp;
}
```
- example usage
```shell
...
      };

      // Client-side listener - for persisting changes to the server
      var modelListener = function(changedModel, options) {
options = options || {};

// Don't persist unless the model is different
if (_.isEqual(JSON.parse(JSON.stringify(model)), JSON.parse(JSON.stringify(model.syncMonitor.get('model'))))) {
  logger.info('modelListener.noChanges', t.className, model.toJSON());
  return;
}

// Disconnect listeners if the ID changes
if (model.get('id') !== modelId) {
  logger.info('modelListener.alteredId', t.className, model.toJSON());
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.pluck"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>pluck (attr)](#apidoc.element.monitor.Backbone.Collection.prototype.pluck)
- description and source-code
```javascript
pluck = function (attr) {
  return _.invoke(this.models, 'get', attr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.pop"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>pop (options)](#apidoc.element.monitor.Backbone.Collection.prototype.pop)
- description and source-code
```javascript
pop = function (options) {
  var model = this.at(this.length - 1);
  this.remove(model, options);
  return model;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.push"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>push (model, options)](#apidoc.element.monitor.Backbone.Collection.prototype.push)
- description and source-code
```javascript
push = function (model, options) {
  model = this._prepareModel(model, options);
  this.add(model, _.extend({at: this.length}, options));
  return model;
}
```
- example usage
```shell
...

// Create an array to hold callbacks for this host
if (!t.addHostCallbacks[hostName]) {
  t.addHostCallbacks[hostName] = [];
}

// Remember this callback and return if we're already adding connections for this host
if (t.addHostCallbacks[hostName].push(callback) > 1) {
  return;
}

// Called when done
var doneAdding = function(error) {
  t.addHostCallbacks[hostName].forEach(function(cb) {
    cb(error);
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.reduce"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>reduce ()](#apidoc.element.monitor.Backbone.Collection.prototype.reduce)
- description and source-code
```javascript
reduce = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>reduceRight ()](#apidoc.element.monitor.Backbone.Collection.prototype.reduceRight)
- description and source-code
```javascript
reduceRight = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.reject"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>reject ()](#apidoc.element.monitor.Backbone.Collection.prototype.reject)
- description and source-code
```javascript
reject = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.remove"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>remove (models, options)](#apidoc.element.monitor.Backbone.Collection.prototype.remove)
- description and source-code
```javascript
remove = function (models, options) {
  var i, l, index, model;
  options || (options = {});
  models = _.isArray(models) ? models.slice() : [models];
  for (i = 0, l = models.length; i < l; i++) {
    model = this.get(models[i]);
    if (!model) continue;
    delete this._byId[model.id];
    delete this._byCid[model.cid];
    index = this.indexOf(model);
    this.models.splice(index, 1);
    this.length--;
    if (!options.silent) {
      options.index = index;
      model.trigger('remove', model, this, options);
    }
    this._removeReference(model);
  }
  return this;
}
```
- example usage
```shell
...
* @protected
* @param connection {Connection} - The connection to remove
*/
removeConnection: function(connection) {
  var t = this;
  log.info('removeConnection', 'Conn_' + connection.id);
  connection.disconnect('connection_removed');
  t.connections.remove(connection);
  t.trigger('connection:remove', connection);
},

/**
* Connect a Monitor object to a remote Probe
*
* This accepts an instance of a Monitor and figures out how to connect it
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.reset"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>reset (models, options)](#apidoc.element.monitor.Backbone.Collection.prototype.reset)
- description and source-code
```javascript
reset = function (models, options) {
  options || (options = {});
  if (options.parse) models = this.parse(models);
  for (var i = 0, l = this.models.length; i < l; i++) {
    this._removeReference(this.models[i]);
  }
  options.previousModels = this.models;
  this._reset();
  if (models) this.add(models, _.extend({silent: true}, options));
  if (!options.silent) this.trigger('reset', this, options);
  return this;
}
```
- example usage
```shell
...
// Call the callback, but don't stop more than once.
if (!t.isListening) {
  return callback();
}

// Release resources
t.connections.each(router.removeConnection, router);
t.connections.reset();

// Shut down the server
t.isListening = false;
server.close();

// Send notices
t.trigger('stop');
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.rest"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>rest ()](#apidoc.element.monitor.Backbone.Collection.prototype.rest)
- description and source-code
```javascript
rest = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.select"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>select ()](#apidoc.element.monitor.Backbone.Collection.prototype.select)
- description and source-code
```javascript
select = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.shift"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>shift (options)](#apidoc.element.monitor.Backbone.Collection.prototype.shift)
- description and source-code
```javascript
shift = function (options) {
  var model = this.at(0);
  this.remove(model, options);
  return model;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.shuffle"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>shuffle ()](#apidoc.element.monitor.Backbone.Collection.prototype.shuffle)
- description and source-code
```javascript
shuffle = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.size"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>size ()](#apidoc.element.monitor.Backbone.Collection.prototype.size)
- description and source-code
```javascript
size = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
...
var newModel = model.syncMonitor.get('model');
if (_.isEqual(JSON.parse(JSON.stringify(model)), JSON.parse(JSON.stringify(newModel)))) {
  logger.info('monitorListener.noChanges', t.className, newModel);
  return;
}

// Disconnect if the model was deleted or the ID isn't the same
var isDeleted = (_.size(newModel) === 0);
if (isDeleted || newModel.id !== modelId)  {
  logger.info('modelListener.deleted', t.className, newModel);
  disconnectListeners();
}

// Forward changes to the model (including server-side delete)
var newOpts = {isSyncChanging:true};
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.slice"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>slice (begin, end)](#apidoc.element.monitor.Backbone.Collection.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  return this.models.slice(begin, end);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.some"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>some ()](#apidoc.element.monitor.Backbone.Collection.prototype.some)
- description and source-code
```javascript
some = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.sort"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>sort (options)](#apidoc.element.monitor.Backbone.Collection.prototype.sort)
- description and source-code
```javascript
sort = function (options) {
  if (!this.comparator) {
    throw new Error('Cannot sort a set without a comparator');
  }

  if (_.isString(this.comparator) || this.comparator.length === 1) {
    this.models = this.sortBy(this.comparator, this);
  } else {
    this.models.sort(_.bind(this.comparator, this));
  }

  if (!options || !options.silent) this.trigger('sort', this, options);
  return this;
}
```
- example usage
```shell
...

  // Allow probes to be externally identified by name
  if (probeJSON.probeName) {
    return probeJSON.probeName;
  }

  if (initParams) {
    _.keys(initParams).sort().forEach(function(key){
      probeKey += ':' + key + '=' + initParams[key];
    });
  }
  return probeKey;
},

/**
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.sortBy"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>sortBy (value, context)](#apidoc.element.monitor.Backbone.Collection.prototype.sortBy)
- description and source-code
```javascript
sortBy = function (value, context) {
  var iterator = _.isFunction(value) ? value : function(model) {
    return model.get(value);
  };
  return _[method](this.models, iterator, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.sortedIndex"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>sortedIndex ()](#apidoc.element.monitor.Backbone.Collection.prototype.sortedIndex)
- description and source-code
```javascript
sortedIndex = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.stopListening"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.Collection.prototype.stopListening)
- description and source-code
```javascript
stopListening = function (object, events, callback) {
  var listeners = this._listeners;
  if (!listeners) return;
  if (object) {
    object.off(events, callback, this);
    if (!events && !callback) delete listeners[object._listenerId];
  } else {
    for (var id in listeners) {
      listeners[id].off(null, null, this);
    }
    this._listeners = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.sync"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>sync ()](#apidoc.element.monitor.Backbone.Collection.prototype.sync)
- description and source-code
```javascript
sync = function () {
  return Backbone.sync.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.tail"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>tail ()](#apidoc.element.monitor.Backbone.Collection.prototype.tail)
- description and source-code
```javascript
tail = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.take"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>take ()](#apidoc.element.monitor.Backbone.Collection.prototype.take)
- description and source-code
```javascript
take = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.toArray"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>toArray ()](#apidoc.element.monitor.Backbone.Collection.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>toJSON (options)](#apidoc.element.monitor.Backbone.Collection.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (options) {
  return this.map(function(model){ return model.toJSON(options); });
}
```
- example usage
```shell
...

The monitor is a [Backbone.js](http://backbonejs.org/) data model so it updates in real time, and you can get all fields with toJSON
():

> processMonitor.get('freemem');
86368256
> processMonitor.get('freemem');
80044032
> processMonitor.toJSON();
...

As the monitor changes, it emits change events:

> processMonitor.on('change', function() {
... console.log(processMonitor.get('freemem'));
... });
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.trigger"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>trigger (name)](#apidoc.element.monitor.Backbone.Collection.prototype.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;
  var args = slice.call(arguments, 1);
  if (!eventsApi(this, 'trigger', name, args)) return this;
  var events = this._events[name];
  var allEvents = this._events.all;
  if (events) triggerEvents(this, events, args);
  if (allEvents) triggerEvents(this, allEvents, arguments);
  return this;
}
```
- example usage
```shell
...

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
},

/**
* Is this connection with the specified host?
*
...
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.unbind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.Collection.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.unshift"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>unshift (model, options)](#apidoc.element.monitor.Backbone.Collection.prototype.unshift)
- description and source-code
```javascript
unshift = function (model, options) {
  model = this._prepareModel(model, options);
  this.add(model, _.extend({at: 0}, options));
  return model;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.update"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>update (models, options)](#apidoc.element.monitor.Backbone.Collection.prototype.update)
- description and source-code
```javascript
update = function (models, options) {
  var model, i, l, existing;
  var add = [], remove = [], modelMap = {};
  var idAttr = this.model.prototype.idAttribute;
  options = _.extend({add: true, merge: true, remove: true}, options);
  if (options.parse) models = this.parse(models);

  // Allow a single model (or no argument) to be passed.
  if (!_.isArray(models)) models = models ? [models] : [];

  // Proxy to 'add' for this case, no need to iterate...
  if (options.add && !options.remove) return this.add(models, options);

  // Determine which models to add and merge, and which to remove.
  for (i = 0, l = models.length; i < l; i++) {
    model = models[i];
    existing = this.get(model.id || model.cid || model[idAttr]);
    if (options.remove && existing) modelMap[existing.cid] = true;
    if ((options.add && !existing) || (options.merge && existing)) {
      add.push(model);
    }
  }
  if (options.remove) {
    for (i = 0, l = this.models.length; i < l; i++) {
      model = this.models[i];
      if (!modelMap[model.cid]) remove.push(model);
    }
  }

  // Remove models (if applicable) before we add and merge the rest.
  if (remove.length) this.remove(remove, options);
  if (add.length) this.add(add, options);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.where"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>where (attrs)](#apidoc.element.monitor.Backbone.Collection.prototype.where)
- description and source-code
```javascript
where = function (attrs) {
  if (_.isEmpty(attrs)) return [];
  return this.filter(function(model) {
    for (var key in attrs) {
      if (attrs[key] !== model.get(key)) return false;
    }
    return true;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Collection.prototype.without"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Collection.prototype.</span>without ()](#apidoc.element.monitor.Backbone.Collection.prototype.without)
- description and source-code
```javascript
without = function () {
  var args = slice.call(arguments);
  args.unshift(this.models);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Backbone.Events"></a>[module monitor.Backbone.Events](#apidoc.module.monitor.Backbone.Events)

#### <a name="apidoc.element.monitor.Backbone.Events.bind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.Events.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
});

// Inbound probe events
t.addEvent('probe:connect', t.probeConnect.bind(t));
t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
t.addEvent('probe:control', t.probeControl.bind(t));

// Connection events
t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
t.addEvent('connection:pong', function(){t.trigger('pong');});
...
```

#### <a name="apidoc.element.monitor.Backbone.Events.listenTo"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.Events.listenTo)
- description and source-code
```javascript
listenTo = function (object, events, callback) {
  var listeners = this._listeners || (this._listeners = {});
  var id = object._listenerId || (object._listenerId = _.uniqueId('l'));
  listeners[id] = object;
  object.on(events, callback || this, this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Events.off"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.Events.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
...
* @method ping
* @param callback {Function(error)} Callback when response is returned
*/
ping: function(callback) {
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
...
```

#### <a name="apidoc.element.monitor.Backbone.Events.on"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.Events.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:

    > processMonitor.on('change', function() {
    ... console.log(processMonitor.get('freemem'));
    ... });

Monitoring your app with a custom script
----------------------------------------

Using Node.js as a scripting language, you can write custom monitors that do anything Node.js can do.  Here's an example that prints
 to the console when free memory falls below a threshold.
...
```

#### <a name="apidoc.element.monitor.Backbone.Events.once"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.Events.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  if (!(eventsApi(this, 'once', name, [callback, context]) && callback)) return this;
  var self = this;
  var once = _.once(function() {
    self.off(name, once);
    callback.apply(this, arguments);
  });
  once._callback = callback;
  this.on(name, once, context);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Events.stopListening"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.Events.stopListening)
- description and source-code
```javascript
stopListening = function (object, events, callback) {
  var listeners = this._listeners;
  if (!listeners) return;
  if (object) {
    object.off(events, callback, this);
    if (!events && !callback) delete listeners[object._listenerId];
  } else {
    for (var id in listeners) {
      listeners[id].off(null, null, this);
    }
    this._listeners = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Events.trigger"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>trigger (name)](#apidoc.element.monitor.Backbone.Events.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;
  var args = slice.call(arguments, 1);
  if (!eventsApi(this, 'trigger', name, args)) return this;
  var events = this._events[name];
  var allEvents = this._events.all;
  if (events) triggerEvents(this, events, args);
  if (allEvents) triggerEvents(this, allEvents, arguments);
  return this;
}
```
- example usage
```shell
...

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
},

/**
* Is this connection with the specified host?
*
...
```

#### <a name="apidoc.element.monitor.Backbone.Events.unbind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Events.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.Events.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Backbone.History"></a>[module monitor.Backbone.History](#apidoc.module.monitor.Backbone.History)

#### <a name="apidoc.element.monitor.Backbone.History.History"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>History ()](#apidoc.element.monitor.Backbone.History.History)
- description and source-code
```javascript
History = function () {
  this.handlers = [];
  _.bindAll(this, 'checkUrl');

  // #1653 - Ensure that 'History' can be used outside of the browser.
  if (typeof window !== 'undefined') {
    this.location = window.location;
    this.history = window.history;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.extend"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.History.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Backbone.History.prototype"></a>[module monitor.Backbone.History.prototype](#apidoc.module.monitor.Backbone.History.prototype)

#### <a name="apidoc.element.monitor.Backbone.History.prototype._updateHash"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>_updateHash (location, fragment, replace)](#apidoc.element.monitor.Backbone.History.prototype._updateHash)
- description and source-code
```javascript
_updateHash = function (location, fragment, replace) {
  if (replace) {
    var href = location.href.replace(/(javascript:|#).*$/, '');
    location.replace(href + '#' + fragment);
  } else {
    // #1649 - Some browsers require that 'hash' contains a leading #.
    location.hash = '#' + fragment;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.bind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
});

// Inbound probe events
t.addEvent('probe:connect', t.probeConnect.bind(t));
t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
t.addEvent('probe:control', t.probeControl.bind(t));

// Connection events
t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
t.addEvent('connection:pong', function(){t.trigger('pong');});
...
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.checkUrl"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>checkUrl (e)](#apidoc.element.monitor.Backbone.History.prototype.checkUrl)
- description and source-code
```javascript
checkUrl = function (e) {
  var current = this.getFragment();
  if (current === this.fragment && this.iframe) {
    current = this.getFragment(this.getHash(this.iframe));
  }
  if (current === this.fragment) return false;
  if (this.iframe) this.navigate(current);
  this.loadUrl() || this.loadUrl(this.getHash());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.getFragment"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>getFragment (fragment, forcePushState)](#apidoc.element.monitor.Backbone.History.prototype.getFragment)
- description and source-code
```javascript
getFragment = function (fragment, forcePushState) {
  if (fragment == null) {
    if (this._hasPushState || !this._wantsHashChange || forcePushState) {
      fragment = this.location.pathname;
      var root = this.root.replace(trailingSlash, '');
      if (!fragment.indexOf(root)) fragment = fragment.substr(root.length);
    } else {
      fragment = this.getHash();
    }
  }
  return fragment.replace(routeStripper, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.getHash"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>getHash (window)](#apidoc.element.monitor.Backbone.History.prototype.getHash)
- description and source-code
```javascript
getHash = function (window) {
  var match = (window || this).location.href.match(/#(.*)$/);
  return match ? match[1] : '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.listenTo"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.History.prototype.listenTo)
- description and source-code
```javascript
listenTo = function (object, events, callback) {
  var listeners = this._listeners || (this._listeners = {});
  var id = object._listenerId || (object._listenerId = _.uniqueId('l'));
  listeners[id] = object;
  object.on(events, callback || this, this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.loadUrl"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>loadUrl (fragmentOverride)](#apidoc.element.monitor.Backbone.History.prototype.loadUrl)
- description and source-code
```javascript
loadUrl = function (fragmentOverride) {
  var fragment = this.fragment = this.getFragment(fragmentOverride);
  var matched = _.any(this.handlers, function(handler) {
    if (handler.route.test(fragment)) {
      handler.callback(fragment);
      return true;
    }
  });
  return matched;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.navigate"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>navigate (fragment, options)](#apidoc.element.monitor.Backbone.History.prototype.navigate)
- description and source-code
```javascript
navigate = function (fragment, options) {
  if (!History.started) return false;
  if (!options || options === true) options = {trigger: options};
  fragment = this.getFragment(fragment || '');
  if (this.fragment === fragment) return;
  this.fragment = fragment;
  var url = this.root + fragment;

  // If pushState is available, we use it to set the fragment as a real URL.
  if (this._hasPushState) {
    this.history[options.replace ? 'replaceState' : 'pushState']({}, document.title, url);

  // If hash changes haven't been explicitly disabled, update the hash
  // fragment to store history.
  } else if (this._wantsHashChange) {
    this._updateHash(this.location, fragment, options.replace);
    if (this.iframe && (fragment !== this.getFragment(this.getHash(this.iframe)))) {
      // Opening and closing the iframe tricks IE7 and earlier to push a
      // history entry on hash-tag change.  When replace is true, we don't
      // want this.
      if(!options.replace) this.iframe.document.open().close();
      this._updateHash(this.iframe.location, fragment, options.replace);
    }

  // If you've told us that you explicitly don't want fallback hashchange-
  // based history, then 'navigate' becomes a page refresh.
  } else {
    return this.location.assign(url);
  }
  if (options.trigger) this.loadUrl(fragment);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.off"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
...
* @method ping
* @param callback {Function(error)} Callback when response is returned
*/
ping: function(callback) {
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
...
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.on"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:

    > processMonitor.on('change', function() {
    ... console.log(processMonitor.get('freemem'));
    ... });

Monitoring your app with a custom script
----------------------------------------

Using Node.js as a scripting language, you can write custom monitors that do anything Node.js can do.  Here's an example that prints
 to the console when free memory falls below a threshold.
...
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.once"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  if (!(eventsApi(this, 'once', name, [callback, context]) && callback)) return this;
  var self = this;
  var once = _.once(function() {
    self.off(name, once);
    callback.apply(this, arguments);
  });
  once._callback = callback;
  this.on(name, once, context);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.route"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>route (route, callback)](#apidoc.element.monitor.Backbone.History.prototype.route)
- description and source-code
```javascript
route = function (route, callback) {
  this.handlers.unshift({route: route, callback: callback});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.start"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>start (options)](#apidoc.element.monitor.Backbone.History.prototype.start)
- description and source-code
```javascript
start = function (options) {
  if (History.started) throw new Error("Backbone.history has already been started");
  History.started = true;

  // Figure out the initial configuration. Do we need an iframe?
  // Is pushState desired ... is it available?
  this.options          = _.extend({}, {root: '/'}, this.options, options);
  this.root             = this.options.root;
  this._wantsHashChange = this.options.hashChange !== false;
  this._wantsPushState  = !!this.options.pushState;
  this._hasPushState    = !!(this.options.pushState && this.history && this.history.pushState);
  var fragment          = this.getFragment();
  var docMode           = document.documentMode;
  var oldIE             = (isExplorer.exec(navigator.userAgent.toLowerCase()) && (!docMode || docMode <= 7));

  // Normalize root to always include a leading and trailing slash.
  this.root = ('/' + this.root + '/').replace(rootStripper, '/');

  if (oldIE && this._wantsHashChange) {
    this.iframe = Backbone.$('<iframe src="javascript:0" tabindex="-1" />').hide().appendTo('body')[0].contentWindow;
    this.navigate(fragment);
  }

  // Depending on whether we're using pushState or hashes, and whether
  // 'onhashchange' is supported, determine how we check the URL state.
  if (this._hasPushState) {
    Backbone.$(window).bind('popstate', this.checkUrl);
  } else if (this._wantsHashChange && ('onhashchange' in window) && !oldIE) {
    Backbone.$(window).bind('hashchange', this.checkUrl);
  } else if (this._wantsHashChange) {
    this._checkUrlInterval = setInterval(this.checkUrl, this.interval);
  }

  // Determine if we need to change the base url, for a pushState link
  // opened by a non-pushState browser.
  this.fragment = fragment;
  var loc = this.location;
  var atRoot = loc.pathname.replace(/[^\/]$/, '$&/') === this.root;

  // If we've started off with a route from a 'pushState'-enabled browser,
  // but we're currently in a browser that doesn't support it...
  if (this._wantsHashChange && this._wantsPushState && !this._hasPushState && !atRoot) {
    this.fragment = this.getFragment(null, true);
    this.location.replace(this.root + this.location.search + '#' + this.fragment);
    // Return immediately as browser will do redirect to new url
    return true;

  // Or if we've started out with a hash-based route, but we're currently
  // in a browser where it could be 'pushState'-based instead...
  } else if (this._wantsPushState && this._hasPushState && atRoot && loc.hash) {
    this.fragment = this.getHash().replace(routeStripper, '');
    this.history.replaceState({}, document.title, this.root + this.fragment + loc.search);
  }

  if (!this.options.silent) return this.loadUrl();
}
```
- example usage
```shell
...

Run the following from your app server directory

    $ npm install monitor

Then place the following line in your application bootstrap, and restart your server

    require('monitor').start();

Monitoring your app with a REPL console
---------------------------------------

Ad-hoc monitoring can be done from a REPL console.

Start up the REPL, and get the Monitor class.  Feel free to copy/paste these lines into your console:
...
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.stop"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>stop ()](#apidoc.element.monitor.Backbone.History.prototype.stop)
- description and source-code
```javascript
stop = function () {
  Backbone.$(window).unbind('popstate', this.checkUrl).unbind('hashchange', this.checkUrl);
  clearInterval(this._checkUrlInterval);
  History.started = false;
}
```
- example usage
```shell
...
server.on('clientError', function(err){
  log.error('bindEvents', 'clientError detected on server', err);
  t.trigger('error', err);
});
server.on('close', function(err){
  server.hasEmittedClose = true;
  log.info('bindEvents.serverClose', 'Server has closed', err);
  t.stop();
});

// Start up the socket.io server.
var socketIoParams = {
  log: false
};
t.socketServer = SocketIO.listen(server, socketIoParams);
...
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.stopListening"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.History.prototype.stopListening)
- description and source-code
```javascript
stopListening = function (object, events, callback) {
  var listeners = this._listeners;
  if (!listeners) return;
  if (object) {
    object.off(events, callback, this);
    if (!events && !callback) delete listeners[object._listenerId];
  } else {
    for (var id in listeners) {
      listeners[id].off(null, null, this);
    }
    this._listeners = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.trigger"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>trigger (name)](#apidoc.element.monitor.Backbone.History.prototype.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;
  var args = slice.call(arguments, 1);
  if (!eventsApi(this, 'trigger', name, args)) return this;
  var events = this._events[name];
  var allEvents = this._events.all;
  if (events) triggerEvents(this, events, args);
  if (allEvents) triggerEvents(this, allEvents, arguments);
  return this;
}
```
- example usage
```shell
...

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
},

/**
* Is this connection with the specified host?
*
...
```

#### <a name="apidoc.element.monitor.Backbone.History.prototype.unbind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.History.prototype.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.History.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Backbone.Model"></a>[module monitor.Backbone.Model](#apidoc.module.monitor.Backbone.Model)

#### <a name="apidoc.element.monitor.Backbone.Model.Model"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>Model (attributes, options)](#apidoc.element.monitor.Backbone.Model.Model)
- description and source-code
```javascript
Model = function (attributes, options) {
  var defaults;
  var attrs = attributes || {};
  this.cid = _.uniqueId('c');
  this.changed = {};
  this.attributes = {};
  this._changes = [];
  if (options && options.collection) this.collection = options.collection;
  if (options && options.parse) attrs = this.parse(attrs);
  if (defaults = _.result(this, 'defaults')) _.defaults(attrs, defaults);
  this.set(attrs, {silent: true});
  this._currentAttributes = _.clone(this.attributes);
  this._previousAttributes = _.clone(this.attributes);
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Model.extend"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Model.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.Model.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Backbone.Router"></a>[module monitor.Backbone.Router](#apidoc.module.monitor.Backbone.Router)

#### <a name="apidoc.element.monitor.Backbone.Router.Router"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>Router (options)](#apidoc.element.monitor.Backbone.Router.Router)
- description and source-code
```javascript
Router = function (options) {
  options || (options = {});
  if (options.routes) this.routes = options.routes;
  this._bindRoutes();
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.extend"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.Router.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Backbone.Router.prototype"></a>[module monitor.Backbone.Router.prototype](#apidoc.module.monitor.Backbone.Router.prototype)

#### <a name="apidoc.element.monitor.Backbone.Router.prototype._bindRoutes"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>_bindRoutes ()](#apidoc.element.monitor.Backbone.Router.prototype._bindRoutes)
- description and source-code
```javascript
_bindRoutes = function () {
  if (!this.routes) return;
  var route, routes = _.keys(this.routes);
  while ((route = routes.pop()) != null) {
    this.route(route, this.routes[route]);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype._extractParameters"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>_extractParameters (route, fragment)](#apidoc.element.monitor.Backbone.Router.prototype._extractParameters)
- description and source-code
```javascript
_extractParameters = function (route, fragment) {
  return route.exec(fragment).slice(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype._routeToRegExp"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>_routeToRegExp (route)](#apidoc.element.monitor.Backbone.Router.prototype._routeToRegExp)
- description and source-code
```javascript
_routeToRegExp = function (route) {
  route = route.replace(escapeRegExp, '\\$&')
               .replace(optionalParam, '(?:$1)?')
               .replace(namedParam, '([^\/]+)')
               .replace(splatParam, '(.*?)');
  return new RegExp('^' + route + '$');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.bind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
});

// Inbound probe events
t.addEvent('probe:connect', t.probeConnect.bind(t));
t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
t.addEvent('probe:control', t.probeControl.bind(t));

// Connection events
t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
t.addEvent('connection:pong', function(){t.trigger('pong');});
...
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>initialize ()](#apidoc.element.monitor.Backbone.Router.prototype.initialize)
- description and source-code
```javascript
initialize = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.listenTo"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.Router.prototype.listenTo)
- description and source-code
```javascript
listenTo = function (object, events, callback) {
  var listeners = this._listeners || (this._listeners = {});
  var id = object._listenerId || (object._listenerId = _.uniqueId('l'));
  listeners[id] = object;
  object.on(events, callback || this, this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.navigate"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>navigate (fragment, options)](#apidoc.element.monitor.Backbone.Router.prototype.navigate)
- description and source-code
```javascript
navigate = function (fragment, options) {
  Backbone.history.navigate(fragment, options);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.off"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
...
* @method ping
* @param callback {Function(error)} Callback when response is returned
*/
ping: function(callback) {
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
...
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.on"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:

    > processMonitor.on('change', function() {
    ... console.log(processMonitor.get('freemem'));
    ... });

Monitoring your app with a custom script
----------------------------------------

Using Node.js as a scripting language, you can write custom monitors that do anything Node.js can do.  Here's an example that prints
 to the console when free memory falls below a threshold.
...
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.once"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  if (!(eventsApi(this, 'once', name, [callback, context]) && callback)) return this;
  var self = this;
  var once = _.once(function() {
    self.off(name, once);
    callback.apply(this, arguments);
  });
  once._callback = callback;
  this.on(name, once, context);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.route"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>route (route, name, callback)](#apidoc.element.monitor.Backbone.Router.prototype.route)
- description and source-code
```javascript
route = function (route, name, callback) {
  if (!_.isRegExp(route)) route = this._routeToRegExp(route);
  if (!callback) callback = this[name];
  Backbone.history.route(route, _.bind(function(fragment) {
    var args = this._extractParameters(route, fragment);
    callback && callback.apply(this, args);
    this.trigger.apply(this, ['route:' + name].concat(args));
    Backbone.history.trigger('route', this, name, args);
  }, this));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.stopListening"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.Router.prototype.stopListening)
- description and source-code
```javascript
stopListening = function (object, events, callback) {
  var listeners = this._listeners;
  if (!listeners) return;
  if (object) {
    object.off(events, callback, this);
    if (!events && !callback) delete listeners[object._listenerId];
  } else {
    for (var id in listeners) {
      listeners[id].off(null, null, this);
    }
    this._listeners = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.trigger"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>trigger (name)](#apidoc.element.monitor.Backbone.Router.prototype.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;
  var args = slice.call(arguments, 1);
  if (!eventsApi(this, 'trigger', name, args)) return this;
  var events = this._events[name];
  var allEvents = this._events.all;
  if (events) triggerEvents(this, events, args);
  if (allEvents) triggerEvents(this, allEvents, arguments);
  return this;
}
```
- example usage
```shell
...

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
},

/**
* Is this connection with the specified host?
*
...
```

#### <a name="apidoc.element.monitor.Backbone.Router.prototype.unbind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.Router.prototype.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.Router.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Backbone.View"></a>[module monitor.Backbone.View](#apidoc.module.monitor.Backbone.View)

#### <a name="apidoc.element.monitor.Backbone.View.View"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.</span>View (options)](#apidoc.element.monitor.Backbone.View.View)
- description and source-code
```javascript
View = function (options) {
  this.cid = _.uniqueId('view');
  this._configure(options || {});
  this._ensureElement();
  this.initialize.apply(this, arguments);
  this.delegateEvents();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.extend"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Backbone.View.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Backbone.View.prototype"></a>[module monitor.Backbone.View.prototype](#apidoc.module.monitor.Backbone.View.prototype)

#### <a name="apidoc.element.monitor.Backbone.View.prototype._configure"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>_configure (options)](#apidoc.element.monitor.Backbone.View.prototype._configure)
- description and source-code
```javascript
_configure = function (options) {
  if (this.options) options = _.extend({}, _.result(this, 'options'), options);
  _.extend(this, _.pick(options, viewOptions));
  this.options = options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype._ensureElement"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>_ensureElement ()](#apidoc.element.monitor.Backbone.View.prototype._ensureElement)
- description and source-code
```javascript
_ensureElement = function () {
  if (!this.el) {
    var attrs = _.extend({}, _.result(this, 'attributes'));
    if (this.id) attrs.id = _.result(this, 'id');
    if (this.className) attrs['class'] = _.result(this, 'className');
    this.setElement(this.make(_.result(this, 'tagName'), attrs), false);
  } else {
    this.setElement(_.result(this, 'el'), false);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.bind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>bind (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
});

// Inbound probe events
t.addEvent('probe:connect', t.probeConnect.bind(t));
t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
t.addEvent('probe:control', t.probeControl.bind(t));

// Connection events
t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
t.addEvent('connection:pong', function(){t.trigger('pong');});
...
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.delegateEvents"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>delegateEvents (events)](#apidoc.element.monitor.Backbone.View.prototype.delegateEvents)
- description and source-code
```javascript
delegateEvents = function (events) {
  if (!(events || (events = _.result(this, 'events')))) return;
  this.undelegateEvents();
  for (var key in events) {
    var method = events[key];
    if (!_.isFunction(method)) method = this[events[key]];
    if (!method) throw new Error('Method "' + events[key] + '" does not exist');
    var match = key.match(delegateEventSplitter);
    var eventName = match[1], selector = match[2];
    method = _.bind(method, this);
    eventName += '.delegateEvents' + this.cid;
    if (selector === '') {
      this.$el.bind(eventName, method);
    } else {
      this.$el.delegate(selector, eventName, method);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>initialize ()](#apidoc.element.monitor.Backbone.View.prototype.initialize)
- description and source-code
```javascript
initialize = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.listenTo"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>listenTo (object, events, callback)](#apidoc.element.monitor.Backbone.View.prototype.listenTo)
- description and source-code
```javascript
listenTo = function (object, events, callback) {
  var listeners = this._listeners || (this._listeners = {});
  var id = object._listenerId || (object._listenerId = _.uniqueId('l'));
  listeners[id] = object;
  object.on(events, callback || this, this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.make"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>make (tagName, attributes, content)](#apidoc.element.monitor.Backbone.View.prototype.make)
- description and source-code
```javascript
make = function (tagName, attributes, content) {
  var el = document.createElement(tagName);
  if (attributes) Backbone.$(el).attr(attributes);
  if (content != null) Backbone.$(el).html(content);
  return el;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.off"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>off (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
...
* @method ping
* @param callback {Function(error)} Callback when response is returned
*/
ping: function(callback) {
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
...
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.on"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>on (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:

    > processMonitor.on('change', function() {
    ... console.log(processMonitor.get('freemem'));
    ... });

Monitoring your app with a custom script
----------------------------------------

Using Node.js as a scripting language, you can write custom monitors that do anything Node.js can do.  Here's an example that prints
 to the console when free memory falls below a threshold.
...
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.once"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>once (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  if (!(eventsApi(this, 'once', name, [callback, context]) && callback)) return this;
  var self = this;
  var once = _.once(function() {
    self.off(name, once);
    callback.apply(this, arguments);
  });
  once._callback = callback;
  this.on(name, once, context);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.remove"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>remove ()](#apidoc.element.monitor.Backbone.View.prototype.remove)
- description and source-code
```javascript
remove = function () {
  this.$el.remove();
  this.stopListening();
  return this;
}
```
- example usage
```shell
...
* @protected
* @param connection {Connection} - The connection to remove
*/
removeConnection: function(connection) {
  var t = this;
  log.info('removeConnection', 'Conn_' + connection.id);
  connection.disconnect('connection_removed');
  t.connections.remove(connection);
  t.trigger('connection:remove', connection);
},

/**
* Connect a Monitor object to a remote Probe
*
* This accepts an instance of a Monitor and figures out how to connect it
...
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.render"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>render ()](#apidoc.element.monitor.Backbone.View.prototype.render)
- description and source-code
```javascript
render = function () {
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.setElement"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>setElement (element, delegate)](#apidoc.element.monitor.Backbone.View.prototype.setElement)
- description and source-code
```javascript
setElement = function (element, delegate) {
  if (this.$el) this.undelegateEvents();
  this.$el = element instanceof Backbone.$ ? element : Backbone.$(element);
  this.el = this.$el[0];
  if (delegate !== false) this.delegateEvents();
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.stopListening"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>stopListening (object, events, callback)](#apidoc.element.monitor.Backbone.View.prototype.stopListening)
- description and source-code
```javascript
stopListening = function (object, events, callback) {
  var listeners = this._listeners;
  if (!listeners) return;
  if (object) {
    object.off(events, callback, this);
    if (!events && !callback) delete listeners[object._listenerId];
  } else {
    for (var id in listeners) {
      listeners[id].off(null, null, this);
    }
    this._listeners = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.trigger"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>trigger (name)](#apidoc.element.monitor.Backbone.View.prototype.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;
  var args = slice.call(arguments, 1);
  if (!eventsApi(this, 'trigger', name, args)) return this;
  var events = this._events[name];
  var allEvents = this._events.all;
  if (events) triggerEvents(this, events, args);
  if (allEvents) triggerEvents(this, allEvents, arguments);
  return this;
}
```
- example usage
```shell
...

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
},

/**
* Is this connection with the specified host?
*
...
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.unbind"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>unbind (name, callback, context)](#apidoc.element.monitor.Backbone.View.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Backbone.View.prototype.undelegateEvents"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.View.prototype.</span>undelegateEvents ()](#apidoc.element.monitor.Backbone.View.prototype.undelegateEvents)
- description and source-code
```javascript
undelegateEvents = function () {
  this.$el.unbind('.delegateEvents' + this.cid);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Backbone.history"></a>[module monitor.Backbone.history](#apidoc.module.monitor.Backbone.history)

#### <a name="apidoc.element.monitor.Backbone.history.checkUrl"></a>[function <span class="apidocSignatureSpan">monitor.Backbone.history.</span>checkUrl ()](#apidoc.element.monitor.Backbone.history.checkUrl)
- description and source-code
```javascript
checkUrl = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Connection"></a>[module monitor.Connection](#apidoc.module.monitor.Connection)

#### <a name="apidoc.element.monitor.Connection.Connection"></a>[function <span class="apidocSignatureSpan">monitor.</span>Connection ()](#apidoc.element.monitor.Connection.Connection)
- description and source-code
```javascript
Connection = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Connection.List"></a>[function <span class="apidocSignatureSpan">monitor.Connection.</span>List ()](#apidoc.element.monitor.Connection.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.Connection.extend"></a>[function <span class="apidocSignatureSpan">monitor.Connection.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Connection.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Connection.List"></a>[module monitor.Connection.List](#apidoc.module.monitor.Connection.List)

#### <a name="apidoc.element.monitor.Connection.List.List"></a>[function <span class="apidocSignatureSpan">monitor.Connection.</span>List ()](#apidoc.element.monitor.Connection.List.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.Connection.List.extend"></a>[function <span class="apidocSignatureSpan">monitor.Connection.List.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Connection.List.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Connection.List.prototype"></a>[module monitor.Connection.List.prototype](#apidoc.module.monitor.Connection.List.prototype)

#### <a name="apidoc.element.monitor.Connection.List.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.Connection.List.prototype.</span>constructor ()](#apidoc.element.monitor.Connection.List.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Connection.List.prototype.model"></a>[function <span class="apidocSignatureSpan">monitor.Connection.List.prototype.</span>model ()](#apidoc.element.monitor.Connection.List.prototype.model)
- description and source-code
```javascript
model = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Connection.prototype"></a>[module monitor.Connection.prototype](#apidoc.module.monitor.Connection.prototype)

#### <a name="apidoc.element.monitor.Connection.prototype.addEvent"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>addEvent (eventName, handler)](#apidoc.element.monitor.Connection.prototype.addEvent)
- description and source-code
```javascript
addEvent = function (eventName, handler) {
  var t = this, socket = t.get('socket');
  t.socketEvents = t.socketEvents || {};
  if (t.socketEvents[eventName]) {
    throw new Error('Event already connected: ' + eventName);
  }
  socket.on(eventName, handler);
  t.socketEvents[eventName] = handler;
  return t;
}
```
- example usage
```shell
...
    */
    bindConnectionEvents: function() {
var t = this, socket = t.get('socket');
if (t.socketEvents) {throw new Error('Already connected');}
t.socketEvents = {};  // key = event name, data = handler

// Failure events
t.addEvent('connect_failed', function(){
  t.trigger('error', 'connect failed');
  t.disconnect('connect failed');
});
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
...
```

#### <a name="apidoc.element.monitor.Connection.prototype.bindConnectionEvents"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>bindConnectionEvents ()](#apidoc.element.monitor.Connection.prototype.bindConnectionEvents)
- description and source-code
```javascript
bindConnectionEvents = function () {
  var t = this, socket = t.get('socket');
  if (t.socketEvents) {throw new Error('Already connected');}
  t.socketEvents = {};  // key = event name, data = handler

  // Failure events
  t.addEvent('connect_failed', function(){
    t.trigger('error', 'connect failed');
    t.disconnect('connect failed');
  });
  t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
  t.addEvent('error', function(reason){
    t.trigger('error', reason);
    t.disconnect('connect error');
  });

  // Inbound probe events
  t.addEvent('probe:connect', t.probeConnect.bind(t));
  t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
  t.addEvent('probe:control', t.probeControl.bind(t));

  // Connection events
  t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
  t.addEvent('connection:pong', function(){t.trigger('pong');});

  // Connected once remote info is known
  t.addEvent('connection:info', function (info) {
    t.set({
      remoteHostName: info.hostName,
      remoteAppName: info.appName,
      remoteAppInstance: info.appInstance,
      remotePID: info.pid,
      remoteProbeClasses: info.probeClasses,
      remoteGateway: info.gateway,
      remoteFirewall: info.firewall
    });
    t.connecting = false;
    t.connected = true;
    t.trigger('connect');
  });

  // Determine the process id
  var pid = typeof process === 'undefined' ? 1 : process.pid;

  // Determine the app instance
  var appInstance = '' + (typeof process === 'undefined' ? pid : process.env.NODE_APP_INSTANCE || pid);

  // Exchange connection information
  socket.emit('connection:info', {
    hostName:Monitor.getRouter().getHostName(),
    appName:Config.Monitor.appName,
    appInstance: appInstance,
    pid: pid,
    probeClasses: _.keys(Probe.classes),
    gateway:t.get('gateway'),
    firewall:t.get('firewall')
  });
}
```
- example usage
```shell
...
t.incomingMonitorsById = {};  // Key = probeId, data = {Monitor proxy}

// Create a connection ID for logging
t.logId = (nextConnectionNum++) + '.';

// Either connect to an URL or with an existing socket
if (params.socket) {
  t.bindConnectionEvents();
  log.info(t.logId + 'connect', {socketId:params.socket.id});
}
else if (params.url || (params.hostName && params.hostPort)) {
  t.connect();
  log.info(t.logId + 'connect', {url:t.get('url')});
}
else {
...
```

#### <a name="apidoc.element.monitor.Connection.prototype.connect"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>connect ()](#apidoc.element.monitor.Connection.prototype.connect)
- description and source-code
```javascript
connect = function () {
  var t = this, hostName = t.get('hostName'), hostPort = t.get('hostPort'),
  url = t.get('url');

  // Build the URL if not specified
  if (!url) {
    url = t.attributes.url = 'http://' + hostName + ':' + hostPort;
    t.set('url', url);
  }

  // Connect with this url
  var opts = {
    // 'transports': ['websocket', 'xhr-polling', 'jsonp-polling'],
    'force new connection': true,      // Don't re-use existing connections
    'reconnect': false                 // Don't let socket.io reconnect.
                                       // Reconnects are performed by the Router.
  };
  var socket = SocketIO.connect(url, opts);
  t.set({socket:socket}).bindConnectionEvents();
}
```
- example usage
```shell
...
undefined

Now connect a monitor to a probe on your app server.  There are a handful of built-in probes, and you can build custom probes for
 your application or npm module.

For this example, we'll monitor the *Process* probe:

> var processMonitor = new Monitor({probeClass:'Process'});
> processMonitor.connect();

The monitor is a [Backbone.js](http://backbonejs.org/) data model so it updates in real time, and you can get all fields with toJSON
():

> processMonitor.get('freemem');
86368256
> processMonitor.get('freemem');
80044032
...
```

#### <a name="apidoc.element.monitor.Connection.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>constructor ()](#apidoc.element.monitor.Connection.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Connection.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>disconnect (reason)](#apidoc.element.monitor.Connection.prototype.disconnect)
- description and source-code
```javascript
disconnect = function (reason) {
  var t = this, socket = t.get('socket');
  t.connecting = false;
  t.connected = false;

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
}
```
- example usage
```shell
...
  t.connected = false;

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
},

/**
* Is this connection with the specified host?
...
```

#### <a name="apidoc.element.monitor.Connection.prototype.emit"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>emit ()](#apidoc.element.monitor.Connection.prototype.emit)
- description and source-code
```javascript
emit = function () {
  var t = this, socket = t.get('socket');
  log.info(t.logId + 'emit', Monitor.deepCopy(arguments, 5));
  socket.emit.apply(socket, arguments);
}
```
- example usage
```shell
...
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
* Disconnect from the remote process
*
* This can be called from the underlying transport if it detects a disconnect,
* or it can be manually called to force a disconnect.
...
```

#### <a name="apidoc.element.monitor.Connection.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>initialize (params)](#apidoc.element.monitor.Connection.prototype.initialize)
- description and source-code
```javascript
initialize = function (params) {
  var t = this;
  t.connecting = true;          // Currently connecting?
  t.connected = false;          // Currently connected?
  t.socketEvents = null;        // Key = event name, data = handler function
  t.remoteProbeIdsByKey = {};   // Key = probeKey, data = probeId
  t.remoteProbesById = {};      // Key = probeId, data = {Probe proxy}
  t.incomingMonitorsById = {};  // Key = probeId, data = {Monitor proxy}

  // Create a connection ID for logging
  t.logId = (nextConnectionNum++) + '.';

  // Either connect to an URL or with an existing socket
  if (params.socket) {
    t.bindConnectionEvents();
    log.info(t.logId + 'connect', {socketId:params.socket.id});
  }
  else if (params.url || (params.hostName && params.hostPort)) {
    t.connect();
    log.info(t.logId + 'connect', {url:t.get('url')});
  }
  else {
    log.error('init', 'Connection must supply a socket, url, or host name/port');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Connection.prototype.isThisHost"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>isThisHost (hostName)](#apidoc.element.monitor.Connection.prototype.isThisHost)
- description and source-code
```javascript
isThisHost = function (hostName) {
  var t = this, testHost = hostName.toLowerCase(),
      myHostName = t.get('hostName'), remoteHostName = t.get('remoteHostName');
  myHostName = myHostName && myHostName.toLowerCase();
  remoteHostName = remoteHostName && remoteHostName.toLowerCase();
  return (testHost === myHostName || testHost ===  remoteHostName);
}
```
- example usage
```shell
...
    * @return connection {Connection} - A Connection object if found, otherwise null
    */
    findConnection: function(hostName, appName, appInstance) {
var t = this, thisInstance = 0;
return t.connections.find(function(conn) {

  // Host or app matches if not specified or if specified and equal
  var matchesHost = !hostName || conn.isThisHost(hostName);
  var matchesApp = !appName || appName === conn.get('remoteAppName');
  var matchesInstance = !appInstance || appInstance === conn.get('remoteAppInstance');
  var remoteFirewall = conn.get('remoteFirewall');

  // This is a match if host + app + instance matches, and it's not firewalled
  return (!remoteFirewall && matchesHost && matchesApp && matchesInstance);
});
...
```

#### <a name="apidoc.element.monitor.Connection.prototype.ping"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>ping (callback)](#apidoc.element.monitor.Connection.prototype.ping)
- description and source-code
```javascript
ping = function (callback) {
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Connection.prototype.probeConnect"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>probeConnect (monitorJSON, callback)](#apidoc.element.monitor.Connection.prototype.probeConnect)
- description and source-code
```javascript
probeConnect = function (monitorJSON, callback) {
  callback = callback || function(){};
  var t = this,
      errorText = '',
      router = Monitor.getRouter(),
      gateway = t.get('gateway'),
      startTime = Date.now(),
      firewall = t.get('firewall'),
      logCtxt = _.extend({}, monitorJSON);

  // Don't allow inbound requests if this connection is firewalled
  if (firewall) {
    errorText = 'firewalled';
    log.error('probeConnect', errorText, logCtxt);
    return callback(errorText);
  }

  // Determine the connection to use (or internal)
  router.determineConnection(monitorJSON, gateway, function(err, connection) {
    if (err) {return callback(err);}
    if (connection && !gateway) {return callback('Not a gateway');}

    // Function to run upon connection (internal or external)
    var onConnect = function(error, probe) {

      if (error) {
        log.error(t.logId + 'probeConnect', error, logCtxt);
        return callback(error);
      }

      // Get probe info
      var probeId = probe.get('id');
      logCtxt.id = probeId;

      // Check for a duplicate proxy for this probeId.  This happens when
      // two connect requests are made before the first one completes.
      var monitorProxy = t.incomingMonitorsById[probeId];
      if (monitorProxy != null) {
        probe.refCount--;
        logCtxt.dupDetected = true;
        logCtxt.refCount = probe.refCount;
        log.info(t.logId + 'probeConnected', logCtxt);
        return callback(null, monitorProxy.probe.toJSON());
      }

      // Connect the montior proxy
      monitorProxy = new Monitor(monitorJSON);
      monitorProxy.set('probeId', probeId);
      t.incomingMonitorsById[probeId] = monitorProxy;
      monitorProxy.probe = probe;
      monitorProxy.probeChange = function(){
        try {
          t.emit('probe:change:' + probeId, probe.changedAttributes());
        }
        catch (e) {
          log.error('probeChange', e, probe, logCtxt);
        }
      };
      probe.connectTime = Date.now();
      var duration = probe.connectTime - startTime;
      logCtxt.duration = duration;
      logCtxt.refCount = probe.refCount;
      log.info(t.logId + 'probeConnected', logCtxt);
      stat.time(t.logId + 'probeConnected', duration);
      callback(null, probe.toJSON());
      probe.on('change', monitorProxy.probeChange);

      // Disconnect the probe on connection disconnect
      t.on('disconnect', function() {
        t.probeDisconnect({probeId:probeId});
      });
    };

    // Connect internally or externally
    if (connection) {
      router.connectExternal(monitorJSON, connection, onConnect);
    } else {
      router.connectInternal(monitorJSON, onConnect);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Connection.prototype.probeControl"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>probeControl (params, callback)](#apidoc.element.monitor.Connection.prototype.probeControl)
- description and source-code
```javascript
probeControl = function (params, callback) {
  callback = callback || function(){};
  var t = this,
      errorText = '',
      logId = t.logId + 'probeControl',
      startTime = Date.now(),
      router = Monitor.getRouter(),
      firewall = t.get('firewall');

  // Don't allow inbound requests if this connection is firewalled
  if (firewall) {
    errorText = 'firewalled';
    log.error(logId, errorText);
    return callback(errorText);
  }

  // Called upon return
  var onReturn = function(error) {
    if (error) {
      log.error(logId, error);
      return callback(error);
    }
    else {
      var duration = Date.now() - startTime;
      log.info(logId + '.return', {duration:duration, returnArgs: arguments});
      stat.time(logId, duration);
      return callback.apply(null, arguments);
    }
  };

  // Is this an internal probe?
  var probe = router.runningProbesById[params.probeId];
  if (!probe) {

    // Is this a remote (proxied) probe?
    var monitorProxy = t.incomingMonitorsById[params.probeId];
    if (!monitorProxy) {
      errorText = 'Probe id not found: ' + params.probeId;
      log.error(errorText);
      return callback(errorText);
    }

    // Proxying requires this form vs. callback as last arg.
    return monitorProxy.control(params.name, params.params, function(err, returnParams) {
      onReturn(err, returnParams);
    });
  }
  logId = logId + '.' + probe.probeClass + '.' + params.name;
  log.info(logId + '.request', {params:params.params, probeId:params.probeId});
  return probe.onControl(params.name, params.params, onReturn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Connection.prototype.probeDisconnect"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>probeDisconnect (params, callback)](#apidoc.element.monitor.Connection.prototype.probeDisconnect)
- description and source-code
```javascript
probeDisconnect = function (params, callback) {
  callback = callback || function(){};
  var t = this,
      errorText = '',
      router = Monitor.getRouter(),
      probeId = params.probeId,
      monitorProxy = t.incomingMonitorsById[probeId],
      firewall = t.get('firewall'),
      logCtxt = null,
      probe = null;

  // Already disconnected
  if (!monitorProxy || !monitorProxy.probe) {
    return callback(null);
  }

  // Get a good logging context
  probe = monitorProxy.probe;
  logCtxt = {
    probeClass: monitorProxy.get('probeClass'),
    initParams: monitorProxy.get('initParams'),
    probeId: probeId
  };

  // Called upon disconnect (internal or external)
  var onDisconnect = function(error) {
    if (error) {
      log.error(t.logId + 'probeDisconnect', error);
      return callback(error);
    }
    var duration = logCtxt.duration = Date.now() - probe.connectTime;
    probe.off('change', monitorProxy.probeChange);
    monitorProxy.probe = monitorProxy.probeChange = null;
    delete t.incomingMonitorsById[probeId];
    log.info(t.logId + 'probeDisconnected', logCtxt);
    stat.time(t.logId + 'probeDisconnected', duration);
    return callback(null);
  };

  // Disconnect from an internal or external probe
  if (probe && probe.connection) {
    router.disconnectExternal(probe.connection, probeId, onDisconnect);
  } else {
    router.disconnectInternal(probeId, onDisconnect);
  }
}
```
- example usage
```shell
...
  log.info(t.logId + 'probeConnected', logCtxt);
  stat.time(t.logId + 'probeConnected', duration);
  callback(null, probe.toJSON());
  probe.on('change', monitorProxy.probeChange);

  // Disconnect the probe on connection disconnect
  t.on('disconnect', function() {
    t.probeDisconnect({probeId:probeId});
  });
};

// Connect internally or externally
if (connection) {
  router.connectExternal(monitorJSON, connection, onConnect);
} else {
...
```

#### <a name="apidoc.element.monitor.Connection.prototype.removeAllEvents"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>removeAllEvents ()](#apidoc.element.monitor.Connection.prototype.removeAllEvents)
- description and source-code
```javascript
removeAllEvents = function () {
  var t = this, socket = t.get('socket');
  for (var event in t.socketEvents) {
    socket.removeListener(event, t.socketEvents[event]);
  }
  t.socketEvents = null;
  return t;
}
```
- example usage
```shell
...
  t.connecting = false;
  t.connected = false;

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
},

/**
...
```

#### <a name="apidoc.element.monitor.Connection.prototype.removeEvent"></a>[function <span class="apidocSignatureSpan">monitor.Connection.prototype.</span>removeEvent (eventName)](#apidoc.element.monitor.Connection.prototype.removeEvent)
- description and source-code
```javascript
removeEvent = function (eventName) {
  var t = this, socket = t.get('socket');
  if (t.socketEvents && t.socketEvents[eventName]) {
    socket.removeListener(eventName, t.socketEvents[eventName]);
    delete t.socketEvents[eventName];
  }
  return t;
}
```
- example usage
```shell
...
  if (!proxy) {return callback('Probe not running');}
  if (--proxy.refCount === 0) {
    // Release probe resources
    proxy.release();
    proxy.connection = null;
    delete connection.remoteProbesById[probeId];
    delete connection.remoteProbeIdsByKey[proxy.probeKey];
    connection.removeEvent('probe:change:' + probeId);
    return connection.emit('probe:disconnect', {probeId:probeId}, function(error){
      return callback(error);
    });
  }
  callback(null);
}
...
```



# <a name="apidoc.module.monitor.Cron"></a>[module monitor.Cron](#apidoc.module.monitor.Cron)

#### <a name="apidoc.element.monitor.Cron.CronJob"></a>[function <span class="apidocSignatureSpan">monitor.Cron.</span>CronJob (cronTime, event, oncomplete)](#apidoc.element.monitor.Cron.CronJob)
- description and source-code
```javascript
function CronJob(cronTime, event, oncomplete) {

  if (!(this instanceof CronJob)) {
    return new CronJob(cronTime, event);
  }

  this.events = [event];
  this.cronTime = new CronTime(cronTime);
  this.now = {};
  this.initiated = false;
  this.oncomplete = oncomplete;

  this.clock();

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Cron.CronTime"></a>[function <span class="apidocSignatureSpan">monitor.Cron.</span>CronTime (time)](#apidoc.element.monitor.Cron.CronTime)
- description and source-code
```javascript
function CronTime(time) {

  this.source = time;

  this.map = ['second', 'minute', 'hour', 'dayOfMonth', 'month', 'dayOfWeek'];
  this.constraints = [[0,59],[0,59],[0,23],[1,31],[0,11],[1,7]];
  this.aliases = {
    jan:0,feb:1,mar:2,apr:3,may:4,jun:5,jul:6,aug:7,sep:8,oct:9,nov:10,dec:11,
    sun:1,mon:2,tue:3,wed:4,thu:5,fri:6,sat:7
  };

  this.second = {};
  this.minute = {};
  this.hour = {};
  this.dayOfMonth = {};
  this.month = {};
  this.dayOfWeek = {};

  this._parse();

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Cron.CronJob"></a>[module monitor.Cron.CronJob](#apidoc.module.monitor.Cron.CronJob)

#### <a name="apidoc.element.monitor.Cron.CronJob.CronJob"></a>[function <span class="apidocSignatureSpan">monitor.Cron.</span>CronJob (cronTime, event, oncomplete)](#apidoc.element.monitor.Cron.CronJob.CronJob)
- description and source-code
```javascript
function CronJob(cronTime, event, oncomplete) {

  if (!(this instanceof CronJob)) {
    return new CronJob(cronTime, event);
  }

  this.events = [event];
  this.cronTime = new CronTime(cronTime);
  this.now = {};
  this.initiated = false;
  this.oncomplete = oncomplete;

  this.clock();

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Cron.CronJob.prototype"></a>[module monitor.Cron.CronJob.prototype](#apidoc.module.monitor.Cron.CronJob.prototype)

#### <a name="apidoc.element.monitor.Cron.CronJob.prototype.addEvent"></a>[function <span class="apidocSignatureSpan">monitor.Cron.CronJob.prototype.</span>addEvent (event)](#apidoc.element.monitor.Cron.CronJob.prototype.addEvent)
- description and source-code
```javascript
addEvent = function (event) {
  this.events.push(event);
}
```
- example usage
```shell
...
    */
    bindConnectionEvents: function() {
var t = this, socket = t.get('socket');
if (t.socketEvents) {throw new Error('Already connected');}
t.socketEvents = {};  // key = event name, data = handler

// Failure events
t.addEvent('connect_failed', function(){
  t.trigger('error', 'connect failed');
  t.disconnect('connect failed');
});
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
...
```

#### <a name="apidoc.element.monitor.Cron.CronJob.prototype.clock"></a>[function <span class="apidocSignatureSpan">monitor.Cron.CronJob.prototype.</span>clock ()](#apidoc.element.monitor.Cron.CronJob.prototype.clock)
- description and source-code
```javascript
clock = function () {

  var date = new Date,
  now = this.now,
  self = this,
  cronTime = this.cronTime,
  i;

  if (!this.initiated) {
    // Make sure we start the clock precisely ON the 0th millisecond
    setTimeout(function(){
                 self.initiated = true;
                 self.clock();
               }, Math.ceil(+date / 1000) * 1000 - +date);
    return;
  }

  this.timer = this.timer || setInterval(function(){self.clock();}, 1000);

  now.second = date.getSeconds();
  now.minute = date.getMinutes();
  now.hour = date.getHours();
  now.dayOfMonth = date.getDate();
  now.month = date.getMonth();
  now.dayOfWeek = date.getDay() + 1;

  for (i in now) {
    if (!(now[i] in cronTime[i])) {
      return;
    }
  }

  this.runEvents();

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Cron.CronJob.prototype.runEvents"></a>[function <span class="apidocSignatureSpan">monitor.Cron.CronJob.prototype.</span>runEvents ()](#apidoc.element.monitor.Cron.CronJob.prototype.runEvents)
- description and source-code
```javascript
runEvents = function () {
  for (var i = -1, l = this.events.length; ++i < l; ) {
    if (typeof this.events[i] === 'function') {
      this.events[i](this.oncomplete);
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Cron.CronTime"></a>[module monitor.Cron.CronTime](#apidoc.module.monitor.Cron.CronTime)

#### <a name="apidoc.element.monitor.Cron.CronTime.CronTime"></a>[function <span class="apidocSignatureSpan">monitor.Cron.</span>CronTime (time)](#apidoc.element.monitor.Cron.CronTime.CronTime)
- description and source-code
```javascript
function CronTime(time) {

  this.source = time;

  this.map = ['second', 'minute', 'hour', 'dayOfMonth', 'month', 'dayOfWeek'];
  this.constraints = [[0,59],[0,59],[0,23],[1,31],[0,11],[1,7]];
  this.aliases = {
    jan:0,feb:1,mar:2,apr:3,may:4,jun:5,jul:6,aug:7,sep:8,oct:9,nov:10,dec:11,
    sun:1,mon:2,tue:3,wed:4,thu:5,fri:6,sat:7
  };

  this.second = {};
  this.minute = {};
  this.hour = {};
  this.dayOfMonth = {};
  this.month = {};
  this.dayOfWeek = {};

  this._parse();

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Cron.CronTime.prototype"></a>[module monitor.Cron.CronTime.prototype](#apidoc.module.monitor.Cron.CronTime.prototype)

#### <a name="apidoc.element.monitor.Cron.CronTime.prototype._parse"></a>[function <span class="apidocSignatureSpan">monitor.Cron.CronTime.prototype.</span>_parse ()](#apidoc.element.monitor.Cron.CronTime.prototype._parse)
- description and source-code
```javascript
_parse = function () {

  var aliases = this.aliases,
  source = this.source.replace(/[a-z]{1,3}/ig, function(alias){

    alias = alias.toLowerCase();

    if (alias in aliases) {
      return aliases[alias];
    }

    throw new Error('Unknown alias: ' + alias);

  }),
  split = source.replace(/^\s\s*|\s\s*$/g, '').split(/\s+/),
  cur, len = 6;

  while (len--) {
    cur = split[len] || '*';
    this._parseField(cur, this.map[len], this.constraints[len]);
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Cron.CronTime.prototype._parseField"></a>[function <span class="apidocSignatureSpan">monitor.Cron.CronTime.prototype.</span>_parseField (field, type, constraints)](#apidoc.element.monitor.Cron.CronTime.prototype._parseField)
- description and source-code
```javascript
_parseField = function (field, type, constraints) {

  var rangePattern = /(\d+?)(?:-(\d+?))?(?:\/(\d+?))?(?:,|$)/g,
  typeObj = this[type],
  diff,
  low = constraints[0],
  high = constraints[1];

  // * is a shortcut to [lower-upper] range
  field = field.replace(/\*/g,  low + '-' + high);

  if (field.match(rangePattern)) {

    field.replace(rangePattern, function($0, lower, upper, step) {

                    step = parseInt(step) || 1;

                    // Positive integer higher than constraints[0]
                    lower = Math.max(low, ~~Math.abs(lower));

                    // Positive integer lower than constraints[1]
                    upper = upper ? Math.min(high, ~~Math.abs(upper)) : lower;

                    // Count from the lower barrier to the upper
                    pointer = lower;

                    do {
                        typeObj[pointer] = true
                        pointer += step;
                    } while(pointer <= upper);

                  });

  } else {

    throw new Error('Field (' + field + ') cannot be parsed');

  }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.DataModelProbe"></a>[module monitor.DataModelProbe](#apidoc.module.monitor.DataModelProbe)

#### <a name="apidoc.element.monitor.DataModelProbe.DataModelProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>DataModelProbe ()](#apidoc.element.monitor.DataModelProbe.DataModelProbe)
- description and source-code
```javascript
DataModelProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.</span>List ()](#apidoc.element.monitor.DataModelProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.DataModelProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.</span>extend (params)](#apidoc.element.monitor.DataModelProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.DataModelProbe.List"></a>[module monitor.DataModelProbe.List](#apidoc.module.monitor.DataModelProbe.List)

#### <a name="apidoc.element.monitor.DataModelProbe.List.List"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.</span>List ()](#apidoc.element.monitor.DataModelProbe.List.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.DataModelProbe.List.extend"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.List.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.DataModelProbe.List.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.DataModelProbe.List.prototype"></a>[module monitor.DataModelProbe.List.prototype](#apidoc.module.monitor.DataModelProbe.List.prototype)

#### <a name="apidoc.element.monitor.DataModelProbe.List.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.List.prototype.</span>constructor ()](#apidoc.element.monitor.DataModelProbe.List.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.List.prototype.model"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.List.prototype.</span>model ()](#apidoc.element.monitor.DataModelProbe.List.prototype.model)
- description and source-code
```javascript
model = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.DataModelProbe.classes"></a>[module monitor.DataModelProbe.classes](#apidoc.module.monitor.DataModelProbe.classes)

#### <a name="apidoc.element.monitor.DataModelProbe.classes.DataModel"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>DataModel ()](#apidoc.element.monitor.DataModelProbe.classes.DataModel)
- description and source-code
```javascript
DataModel = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.classes.File"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>File ()](#apidoc.element.monitor.DataModelProbe.classes.File)
- description and source-code
```javascript
File = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.classes.FileSyncProbe"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>FileSyncProbe ()](#apidoc.element.monitor.DataModelProbe.classes.FileSyncProbe)
- description and source-code
```javascript
FileSyncProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.classes.Inspect"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Inspect ()](#apidoc.element.monitor.DataModelProbe.classes.Inspect)
- description and source-code
```javascript
Inspect = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.classes.Log"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Log ()](#apidoc.element.monitor.DataModelProbe.classes.Log)
- description and source-code
```javascript
Log = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.classes.Process"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Process ()](#apidoc.element.monitor.DataModelProbe.classes.Process)
- description and source-code
```javascript
Process = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.classes.Recipe"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Recipe ()](#apidoc.element.monitor.DataModelProbe.classes.Recipe)
- description and source-code
```javascript
Recipe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.classes.Repl"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Repl ()](#apidoc.element.monitor.DataModelProbe.classes.Repl)
- description and source-code
```javascript
Repl = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.classes.Stat"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Stat ()](#apidoc.element.monitor.DataModelProbe.classes.Stat)
- description and source-code
```javascript
Stat = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.DataModelProbe.classes.Sync"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.classes.</span>Sync ()](#apidoc.element.monitor.DataModelProbe.classes.Sync)
- description and source-code
```javascript
Sync = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
* functionality to any Backbone data model.
*
* The returned function can be assigned to the '''sync''' element when defining the
* data model:
*
*     var BlogEntry = Backbone.Model.extend({
*       ...
*       sync: Monitor.Sync('BlogEntry'),
*       ...
*     });
*
* The sync function can also be assigned to any Backbone model after construction:
*
*     var myBook = new Book({id:"44329"});
*     myBook.sync = Monitor.Sync('Book');
...
```



# <a name="apidoc.module.monitor.DataModelProbe.prototype"></a>[module monitor.DataModelProbe.prototype](#apidoc.module.monitor.DataModelProbe.prototype)

#### <a name="apidoc.element.monitor.DataModelProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.DataModelProbe.prototype.</span>constructor ()](#apidoc.element.monitor.DataModelProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.FileProbe"></a>[module monitor.FileProbe](#apidoc.module.monitor.FileProbe)

#### <a name="apidoc.element.monitor.FileProbe.FileProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>FileProbe ()](#apidoc.element.monitor.FileProbe.FileProbe)
- description and source-code
```javascript
FileProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.</span>List ()](#apidoc.element.monitor.FileProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.FileProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.</span>extend (params)](#apidoc.element.monitor.FileProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```

#### <a name="apidoc.element.monitor.FileProbe.getRootPath"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.</span>getRootPath ()](#apidoc.element.monitor.FileProbe.getRootPath)
- description and source-code
```javascript
getRootPath = function () {
  return ROOT_PATH;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe.mkdir_r"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.</span>mkdir_r (dirname, mode, callback)](#apidoc.element.monitor.FileProbe.mkdir_r)
- description and source-code
```javascript
mkdir_r = function (dirname, mode, callback) {

  // Optional arguments
  if (typeof mode === 'function') {
    callback = mode;
    mode = null;
  }
  callback = callback || function(){};
  mode = mode || '777';

  // First attempt
  FS.mkdir(dirname, mode, function(err1) {

    // Success
    if (!err1 || err1.code === 'EEXIST') {
      return callback(null);
    }

    // Failure.  Try making parent.
    var parent = Path.dirname(dirname);
    FileProbe.mkdir_r(parent, mode, function(err2) {

      // Successful parent create.  Try child one more time.
      if (!err2) {
        return FS.mkdir(dirname, mode, callback);
      }

      // Couldn't make parent.
      callback(err2);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe.rm_rf"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.</span>rm_rf (path, callback)](#apidoc.element.monitor.FileProbe.rm_rf)
- description and source-code
```javascript
rm_rf = function (path, callback) {

  // Get the file/dir status
  callback = callback || function(){};
  var stats = FS.lstat(path, function(err, stats){
    if (err) {
      return callback(err);
    }

    // If it's a directory, remove all files then the directory
    if (stats.isDirectory()) {

      // Read all files in the directory
      FS.readdir(path, function(err1, files) {
        if (err1) {
          return callback(err1);
        }

        // Done if no files
        if (files.length === 0) {
          return callback();
        }

        // Remove all files asynchronously
        var numLeft = files.length;
        var lastError = null;
        files.forEach(function (filename) {
          FileProbe.rm_rf(Path.join(path, filename), function(err2){
            lastError = err2 || lastError;
            if (--numLeft === 0) {
              if (lastError) {
                return callback(lastError);
              }
              // Remove the original directory
              FS.rmdir(path, callback);
            }
          });
        });
      });
    }

    // Directly remove if it's any non-directory type
    else {
      return FS.unlink(path, callback);
    }

  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe.setRootPath"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.</span>setRootPath (rootPath)](#apidoc.element.monitor.FileProbe.setRootPath)
- description and source-code
```javascript
setRootPath = function (rootPath) {
  var normalized = Path.normalize(rootPath);
  if (ROOT_PATH && ROOT_PATH !== normalized) {
    throw new Error('Cannot change the File probe root path once set.');
  }
  ROOT_PATH = normalized;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe.tail"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.</span>tail ()](#apidoc.element.monitor.FileProbe.tail)
- description and source-code
```javascript
tail = function () {
  var t = this, path = t.fullPath;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe.watch"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.</span>watch (path, options, callback)](#apidoc.element.monitor.FileProbe.watch)
- description and source-code
```javascript
watch = function (path, options, callback) {

  // Process arguments
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  var defaultOpts = {persistent:false, pollStyle:false, interval:10};
  var opts = _.extend({}, defaultOpts, options);

  // Use fs.watch or fs.watchFile
  var watcher = null;
  if (FS.watch && !opts.pollStyle) {
    // Latest watch method
    try {
      watcher = FS.watch(path, opts, function(event, filename) {
        callback(event);
      });
    } catch (e) {
      // Return a mock watcher.  The callback will be called on error.
      watcher = {
        close: function(){}
      };
    }
  }
  else {
    FS.watchFile(path, opts, function(curr, prev) {
      // Detect file deletion
      if (curr.nlink === 0) {
        return callback('rename');
      }
      if (curr.mtime.getTime() === prev.mtime.getTime()) {
        return;
      }
      return callback('change');
    });
  }

  // Return the object for closing
  return {
    close: function() {
      if (watcher) {
        watcher.close();
      } else {
        FS.unwatchFile(path);
      }
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe.watchLoad"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.</span>watchLoad (path, options, callback)](#apidoc.element.monitor.FileProbe.watchLoad)
- description and source-code
```javascript
watchLoad = function (path, options, callback) {

  // Process arguments
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  var defaultOpts = {encoding:'utf8', preload:false, persistent:false};
  var opts = _.extend({}, defaultOpts, options);

  // Build the function to call when the file changes
  var onFileChange = function() {
    FS.readFile(path, options.encoding, function(err, text) {
      if (err) {
        // Forward the error
        return callback(err);
      }
      // Success
      callback(null, text.toString());
    });
  };

  // Read initial file contents if requested
  if (options.preload) {
    onFileChange();
  }

  // Connect the file watcher
  return FileProbe.watch(path, options, onFileChange);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.FileProbe.prototype"></a>[module monitor.FileProbe.prototype](#apidoc.module.monitor.FileProbe.prototype)

#### <a name="apidoc.element.monitor.FileProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.prototype.</span>constructor ()](#apidoc.element.monitor.FileProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.FileProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (attributes, options){
  var t = this;
  Probe.prototype.initialize.apply(t, arguments);

  // Disable the probe if the root path hasn't been set
  if (!ROOT_PATH) {
    throw new Error('File probe has not been enabled on this server.');
  }

  // Don't allow a path above the root path
  t.fullPath = Path.join(ROOT_PATH, t.get('path'));
  if (t.fullPath.indexOf(ROOT_PATH) !== 0) {
    throw new Error('Invalid file path');
  }

  // Assume callback responsibility.
  options.asyncInit = true;
  var callback = options.callback;

  // Set up for reading or tailing
  if (t.get('tail')) {

    //TODO: Implement tail
    return callback({code:'UNDER_CONSTRUCTION', msg:'Tail functionality not implemented.'});

  } else {

    // Build the function to call on initial load and subsequent change
    t.onLoad = function(error, newContent) {
      var firstLoad = (callback !== null);
      t.set({error: error, text: newContent}, {silent:firstLoad});

      // Call the init callback on first load
      if (firstLoad) {
        callback(error);
        callback = null;
      }
    };

    // Load and watch the file
    var watcherOpts = {
      preload: true,
      persistent: true
    };
    t.watcher = FileProbe.watchLoad(t.fullPath, watcherOpts, t.onLoad);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.FileProbe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.FileProbe.prototype.</span>release ()](#apidoc.element.monitor.FileProbe.prototype.release)
- description and source-code
```javascript
release = function () {
  var t = this;
  if (t.watcher) {
    t.watcher.close();
  }
  Probe.prototype.release.apply(t, arguments);
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```



# <a name="apidoc.module.monitor.InspectProbe"></a>[module monitor.InspectProbe](#apidoc.module.monitor.InspectProbe)

#### <a name="apidoc.element.monitor.InspectProbe.InspectProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>InspectProbe ()](#apidoc.element.monitor.InspectProbe.InspectProbe)
- description and source-code
```javascript
InspectProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.InspectProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.InspectProbe.</span>List ()](#apidoc.element.monitor.InspectProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.InspectProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.InspectProbe.</span>extend (params)](#apidoc.element.monitor.InspectProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.InspectProbe.prototype"></a>[module monitor.InspectProbe.prototype](#apidoc.module.monitor.InspectProbe.prototype)

#### <a name="apidoc.element.monitor.InspectProbe.prototype._evaluate"></a>[function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>_evaluate (expression)](#apidoc.element.monitor.InspectProbe.prototype._evaluate)
- description and source-code
```javascript
_evaluate = function (expression){
  var t = this,
      value = null;

  // Evaluate the expression
  try {
    value = eval(expression);
  } catch (e) {
    var err = 'Unable to evaluate expression: "' + expression + '"';
    logger.error('evaluate', err);
    throw new Error(err);
  }

  // Return the value
  return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.InspectProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>constructor ()](#apidoc.element.monitor.InspectProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.InspectProbe.prototype.eval_control"></a>[function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>eval_control (expression, depth)](#apidoc.element.monitor.InspectProbe.prototype.eval_control)
- description and source-code
```javascript
eval_control = function (expression, depth){
  var t = this;

  // Determine a default depth
  depth = typeof depth === 'undefined' ? DEFAULT_DEPTH : depth;

  // Get the raw value
  var value = t._evaluate(expression);

  // Return the depth limited results
  return Monitor.deepCopy(value, depth);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.InspectProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>initialize (initParams)](#apidoc.element.monitor.InspectProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (initParams){
  var t = this;

  // Get the global object if the key isn't specified
  t.key = initParams.key;
  if (typeof initParams.key === 'undefined') {
    t.key = typeof window === 'undefined' ? 'global' : 'window';
  }

  // Get a good depth default.  Default unless key = window.
  if (typeof initParams.depth === 'undefined') {
    if (!initParams.key && t.key === 'window') {
      t.depth = 1;
    } else {
      t.depth = DEFAULT_DEPTH;
    }
  } else {
    t.depth = initParams.depth;
  }

  // Evaluate the expression to see if it's a Backbone.Model
  // This will throw an exception if the key is a bad expression
  t.value = t._evaluate(t.key);
  t.isModel = t.value instanceof Backbone.Model;

  // Set the initial values
  t.set({
    value: Monitor.deepCopy(t.value, t.depth),
    isModel: t.isModel
  });

  // Watch for backbone model changes, or initialize the polling probe
  if (t.isModel) {
    t.value.on('change', t.poll, t);
  } else {
    PollingProbe.prototype.initialize.apply(t, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.InspectProbe.prototype.poll"></a>[function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>poll ()](#apidoc.element.monitor.InspectProbe.prototype.poll)
- description and source-code
```javascript
poll = function () {
  var t = this,
      newValue = t.eval_control(t.key, t.depth);

  // Set the new value if it has changed from the current value
  if (!_.isEqual(newValue, t.get('value'))) {
    t.set({value: newValue});
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.InspectProbe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>release ()](#apidoc.element.monitor.InspectProbe.prototype.release)
- description and source-code
```javascript
release = function () {
  var t = this;
  if (t.isModel) {
    t.value.off('change', t.poll, t);
  } else {
    PollingProbe.prototype.release.apply(t, arguments);
  }
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```

#### <a name="apidoc.element.monitor.InspectProbe.prototype.set_control"></a>[function <span class="apidocSignatureSpan">monitor.InspectProbe.prototype.</span>set_control (attrs, callback)](#apidoc.element.monitor.InspectProbe.prototype.set_control)
- description and source-code
```javascript
set_control = function (attrs, callback) {
  var t = this;

  // Value is the only thing to set
  if (typeof attrs.value === 'undefined') {
    return callback({code:'NO_VALUE'});
  }

  // Set the model elements.  These cause change events to fire
  if (t.isModel) {
    t.value.set(attrs.value);
  }
  else {
    // Set the variable directly
    var jsonValue = JSON.stringify(attrs.value);
    t._evaluate(t.key + ' = ' + jsonValue);
    t.set('value', attrs.value);
  }
  return callback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.List"></a>[module monitor.List](#apidoc.module.monitor.List)

#### <a name="apidoc.element.monitor.List.List"></a>[function <span class="apidocSignatureSpan">monitor.</span>List ()](#apidoc.element.monitor.List.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.List.extend"></a>[function <span class="apidocSignatureSpan">monitor.List.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.List.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.List.prototype"></a>[module monitor.List.prototype](#apidoc.module.monitor.List.prototype)

#### <a name="apidoc.element.monitor.List.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.List.prototype.</span>constructor ()](#apidoc.element.monitor.List.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.List.prototype.model"></a>[function <span class="apidocSignatureSpan">monitor.List.prototype.</span>model ()](#apidoc.element.monitor.List.prototype.model)
- description and source-code
```javascript
model = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Log"></a>[module monitor.Log](#apidoc.module.monitor.Log)

#### <a name="apidoc.element.monitor.Log.Log"></a>[function <span class="apidocSignatureSpan">monitor.</span>Log (module)](#apidoc.element.monitor.Log.Log)
- description and source-code
```javascript
Log = function (module) {
  var t = this;
  t.module = module;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log._emit"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>_emit (type, module, name, args)](#apidoc.element.monitor.Log._emit)
- description and source-code
```javascript
_emit = function (type, module, name, args) {
  var eventName,
      fullName = type + '.' + module + '.' + name;

  // Prevent log recursion. This has the effect of disabling all logging
  // for log handlers (and their downstream effect), but is necessary to
  // prevent infinite recursion.  If it's desired to log the output of
  // log handlers, then delay that processing until nextTick.
  if (emittingNow) {
    return;
  }
  emittingNow = true;

  // Output a counter stat for this log
  stat.increment(fullName);

  // Test the name against all registered events
  for (eventName in Log._events) {

    // Get the regex associated with the name (using the Stat package)
    var regex = Log.eventRegex[eventName];
    if (!regex) {
      regex = Log.eventRegex[eventName] = Stat._buildRegex(eventName);
    }

    // Test the long name with the regex, and emit if it matches
    if (regex.test(fullName)) {

      // Build the arguments as event name, log type, module, name, [other args...]
      var allArgs = _.toArray(args),
          emitFn = Log.emit || Log.trigger; // NodeJS/server=emit, Backbone/browser=trigger
      allArgs.splice(0, 1, eventName, type, module, name);
      emitFn.apply(Log, allArgs);
    }
  }

  // Turn off recursion prevention
  emittingNow = false;
}
```
- example usage
```shell
...
*
* @method increment
* @param name {String} Dot.separated name of the counter to increment
* @param [value=1] {Number} Amount to increment the counter by.
*/
proto.increment = function(name, value){
  value = _.isNumber(value) ? value : 1;
  Stat._emit(this.module, name, value, 'c');
};

/**
* Decrement a counter by a specified value
*
* Assuming someone is listening to this stat, this is an instruction for that
* listener to subtract the specified value (usually 1) to their prior value for this stat.
...
```

#### <a name="apidoc.element.monitor.Log.addListener"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>addListener (type, listener)](#apidoc.element.monitor.Log.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.console"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>console (type, module, name)](#apidoc.element.monitor.Log.console)
- description and source-code
```javascript
console = function (type, module, name) {

  // Build the string to log, in log4js format
  var nowStr = (new Date()).toJSON(),
      args = _.toArray(arguments),
      logStr = '[' + nowStr + '] [' + type.toUpperCase() + '] ' + module;

  // Remove the type, module, name leaving the args to the log
  args.splice(0,3);

  // If no args, then they didn't provide a name
  if (args.length === 0) {
    args = [name];
  }
  else {
    // Add the log entry name
    logStr += '.' + name;
  }

  // If the output is simple, just print it.  Otherwise JSON.stringify it.
  logStr += ' - ';
  if (args.length === 1 && typeof args[0] === 'string') {
    logStr += args[0];
  }
  else {
    try {
      logStr += JSON.stringify(args);
    } catch(e) {
      logStr += Monitor.stringify(args);
    }
  }

  // Send to the console - Log or error
  if (type === 'error' || type === 'fatal') {
    console.error(logStr);
  }
  else {
    console.log(logStr);
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.emit"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>emit (type)](#apidoc.element.monitor.Log.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
...
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
* Disconnect from the remote process
*
* This can be called from the underlying transport if it detects a disconnect,
* or it can be manually called to force a disconnect.
...
```

#### <a name="apidoc.element.monitor.Log.eventNames"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>eventNames ()](#apidoc.element.monitor.Log.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.getMaxListeners"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>getMaxListeners ()](#apidoc.element.monitor.Log.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.listenerCount"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>listenerCount (type)](#apidoc.element.monitor.Log.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.listeners"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>listeners (type)](#apidoc.element.monitor.Log.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.on"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>on (type, listener)](#apidoc.element.monitor.Log.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:

    > processMonitor.on('change', function() {
    ... console.log(processMonitor.get('freemem'));
    ... });

Monitoring your app with a custom script
----------------------------------------

Using Node.js as a scripting language, you can write custom monitors that do anything Node.js can do.  Here's an example that prints
 to the console when free memory falls below a threshold.
...
```

#### <a name="apidoc.element.monitor.Log.once"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>once (type, listener)](#apidoc.element.monitor.Log.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.prependListener"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>prependListener (type, listener)](#apidoc.element.monitor.Log.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.prependOnceListener"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>prependOnceListener (type, listener)](#apidoc.element.monitor.Log.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.removeAllListeners"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>removeAllListeners (type)](#apidoc.element.monitor.Log.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.removeListener"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>removeListener (type, listener)](#apidoc.element.monitor.Log.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
...
  return t;
},

// Remove the specified event from the socket
removeEvent: function(eventName) {
  var t = this, socket = t.get('socket');
  if (t.socketEvents && t.socketEvents[eventName]) {
    socket.removeListener(eventName, t.socketEvents[eventName]);
    delete t.socketEvents[eventName];
  }
  return t;
},

// Remove all events bound to the socket
removeAllEvents: function() {
...
```

#### <a name="apidoc.element.monitor.Log.setMaxListeners"></a>[function <span class="apidocSignatureSpan">monitor.Log.</span>setMaxListeners (n)](#apidoc.element.monitor.Log.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Log._events"></a>[module monitor.Log._events](#apidoc.module.monitor.Log._events)



# <a name="apidoc.module.monitor.Log.prototype"></a>[module monitor.Log.prototype](#apidoc.module.monitor.Log.prototype)

#### <a name="apidoc.element.monitor.Log.prototype.debug"></a>[function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>debug (name)](#apidoc.element.monitor.Log.prototype.debug)
- description and source-code
```javascript
debug = function (name) {
  Log._emit(method, this.module, name, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.prototype.error"></a>[function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>error (name)](#apidoc.element.monitor.Log.prototype.error)
- description and source-code
```javascript
error = function (name) {
  Log._emit(method, this.module, name, arguments);
}
```
- example usage
```shell
...
        console.log('Low memory warning: ' + freemem);
      }
    });

    // Now connect the monitor
    processMonitor.connect(function(error) {
      if (error) {
        console.error('Error connecting with the process probe: ', error);
        process.exit(1);
      }
    });

Monitoring your app in a browser
--------------------------------
...
```

#### <a name="apidoc.element.monitor.Log.prototype.fatal"></a>[function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>fatal (name)](#apidoc.element.monitor.Log.prototype.fatal)
- description and source-code
```javascript
fatal = function (name) {
  Log._emit(method, this.module, name, arguments);
}
```
- example usage
```shell
...
// On laptop sleep/startup the DNS servers aren't immediately available,
// resulting in a flood of these for socket.io until DNS services are back up.
if (err.message === 'ECONNREFUSED, Could not contact DNS servers') {
  return;
}

// Don't allow the process to continue in an unknown state.
log.fatal('moniotor.uncaught', 'Uncaught Exception: ' + err.message);
log.fatal('moniotor.uncaught', err.stack);
server.stop(function(){
  process.exit(1);
});

// Don't wait around if the server is hung.
setTimeout(function(){process.exit(1);}, 2000);
...
```

#### <a name="apidoc.element.monitor.Log.prototype.info"></a>[function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>info (name)](#apidoc.element.monitor.Log.prototype.info)
- description and source-code
```javascript
info = function (name) {
  Log._emit(method, this.module, name, arguments);
}
```
- example usage
```shell
...

// Create a connection ID for logging
t.logId = (nextConnectionNum++) + '.';

// Either connect to an URL or with an existing socket
if (params.socket) {
  t.bindConnectionEvents();
  log.info(t.logId + 'connect', {socketId:params.socket.id});
}
else if (params.url || (params.hostName && params.hostPort)) {
  t.connect();
  log.info(t.logId + 'connect', {url:t.get('url')});
}
else {
  log.error('init', 'Connection must supply a socket, url, or host name/port');
...
```

#### <a name="apidoc.element.monitor.Log.prototype.trace"></a>[function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>trace (name)](#apidoc.element.monitor.Log.prototype.trace)
- description and source-code
```javascript
trace = function (name) {
  Log._emit(method, this.module, name, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Log.prototype.warn"></a>[function <span class="apidocSignatureSpan">monitor.Log.prototype.</span>warn (name)](#apidoc.element.monitor.Log.prototype.warn)
- description and source-code
```javascript
warn = function (name) {
  Log._emit(method, this.module, name, arguments);
}
```
- example usage
```shell
...
    }
  }

  // Set the data
  var error = null;
  if (!t.set(attrs)) {
    error = {code:'VALIDATION_ERROR', msg:'Data set failed validation'};
    log.warn('set_control', error);
  }
  return callback(error);
},

/**
* Respond to a ping control sent from a monitor
*
...
```



# <a name="apidoc.module.monitor.LogProbe"></a>[module monitor.LogProbe](#apidoc.module.monitor.LogProbe)

#### <a name="apidoc.element.monitor.LogProbe.LogProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>LogProbe ()](#apidoc.element.monitor.LogProbe.LogProbe)
- description and source-code
```javascript
LogProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.LogProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.LogProbe.</span>List ()](#apidoc.element.monitor.LogProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.LogProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.LogProbe.</span>extend (params)](#apidoc.element.monitor.LogProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.LogProbe.prototype"></a>[module monitor.LogProbe.prototype](#apidoc.module.monitor.LogProbe.prototype)

#### <a name="apidoc.element.monitor.LogProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.LogProbe.prototype.</span>constructor ()](#apidoc.element.monitor.LogProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.LogProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.LogProbe.prototype.</span>initialize ()](#apidoc.element.monitor.LogProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (){
  var t = this;

  // Call parent constructor
  StreamProbe.prototype.initialize.apply(t, arguments);

  // The watcher just forwards all args to queueItem as an array
  t.watcher = function() {
    // Add timestamp as the first element
    var logElems = _.toArray(arguments);
    logElems.splice(0,0,JSON.stringify(new Date()).substr(1,24));
    t.queueItem.call(t, logElems);
  };
  Log.on(t.get('pattern'), t.watcher);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.LogProbe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.LogProbe.prototype.</span>release ()](#apidoc.element.monitor.LogProbe.prototype.release)
- description and source-code
```javascript
release = function () {
  var t = this;
  Log.off(t.get('pattern'), t.watcher);
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```



# <a name="apidoc.module.monitor.PollingProbe"></a>[module monitor.PollingProbe](#apidoc.module.monitor.PollingProbe)

#### <a name="apidoc.element.monitor.PollingProbe.PollingProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>PollingProbe ()](#apidoc.element.monitor.PollingProbe.PollingProbe)
- description and source-code
```javascript
PollingProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.PollingProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.PollingProbe.</span>List ()](#apidoc.element.monitor.PollingProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.PollingProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.PollingProbe.</span>extend (params)](#apidoc.element.monitor.PollingProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.PollingProbe.prototype"></a>[module monitor.PollingProbe.prototype](#apidoc.module.monitor.PollingProbe.prototype)

#### <a name="apidoc.element.monitor.PollingProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.PollingProbe.prototype.</span>constructor ()](#apidoc.element.monitor.PollingProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.PollingProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.PollingProbe.prototype.</span>initialize ()](#apidoc.element.monitor.PollingProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (){
  var t = this,
      pollInterval = t.get('pollInterval'),
      cronPattern = t.get('cronPattern'),
      poll = function(){t.poll();};
  Probe.prototype.initialize.apply(t, arguments);

  // Override cron for the default 1-second interval
  // (this allows the default to work when Cron isn't available)
  if (pollInterval == null && cronPattern === DEFAULT_CRON_PATTERN) {
    pollInterval = DEFAULT_POLL_INTERVAL;
  }

  // Poll once, then set up the interval
  t.poll();
  if (pollInterval !== 0) {
    if (pollInterval) {
      t.timer = setInterval(poll, pollInterval);
    } else {
      if (!Cron) {
        throw new Error("Cron is not available in this client");
      }
      t.cronJob = new Cron.CronJob(cronPattern, poll);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.PollingProbe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.PollingProbe.prototype.</span>release ()](#apidoc.element.monitor.PollingProbe.prototype.release)
- description and source-code
```javascript
release = function (){
  var t = this, timer = (t.cronJob ? t.cronJob.timer : t.timer);
  if (t.cronJob && !t.cronJob.initiated) {
    // If cron isn't initiated we've been asked to shut down within the
    // first second, and the timer hasn't been set (but will be soon).
    setTimeout(function(){clearInterval(t.cronJob.timer);}, 1000);
  } else if (t.timer) {
    clearInterval(timer);
  }
  t.timer = t.cron = null;
  Probe.prototype.release.apply(t, arguments);
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```



# <a name="apidoc.module.monitor.Probe"></a>[module monitor.Probe](#apidoc.module.monitor.Probe)

#### <a name="apidoc.element.monitor.Probe.Probe"></a>[function <span class="apidocSignatureSpan">monitor.</span>Probe ()](#apidoc.element.monitor.Probe.Probe)
- description and source-code
```javascript
Probe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Probe.List"></a>[function <span class="apidocSignatureSpan">monitor.Probe.</span>List ()](#apidoc.element.monitor.Probe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.Probe.extend"></a>[function <span class="apidocSignatureSpan">monitor.Probe.</span>extend (params)](#apidoc.element.monitor.Probe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Probe.prototype"></a>[module monitor.Probe.prototype](#apidoc.module.monitor.Probe.prototype)

#### <a name="apidoc.element.monitor.Probe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>constructor ()](#apidoc.element.monitor.Probe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Probe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.Probe.prototype.initialize)
- description and source-code
```javascript
initialize = function (attributes, options) {
  var t = this;
  log.info('init', t.toJSON(), options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Probe.prototype.onControl"></a>[function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>onControl (name, params, callback)](#apidoc.element.monitor.Probe.prototype.onControl)
- description and source-code
```javascript
onControl = function (name, params, callback) {
  var t = this,
      controlFn = t[name + '_control'],
      startTime = Date.now(),
      errMsg,
      logId = 'onControl.' + t.probeClass + '.' + name;

  params = params || {};
  callback = callback || function(){};
  log.info(logId, t.get('id'), params);

  if (!controlFn) {
    errMsg = 'No control function: ' + name;
    log.error(logId, errMsg);
    return callback({msg: errMsg});
  }

  var whenDone = function(error) {
    if (error) {
      log.error(logId + '.whenDone', error);
      return callback(error);
    }
    var duration = Date.now() - startTime;
    log.info(logId, params);
    stat.time(t.logId, duration);
    callback.apply(null, arguments);
  };

  // Run the control on next tick.  This provides a consistent callback
  // chain for local and remote probes.
  setTimeout(function(){
    try {
      controlFn.call(t, params, whenDone);
    } catch (e) {
      errMsg = 'Error calling control: ' + t.probeClass + ':' + name;
      whenDone({msg:errMsg, err: e.toString()});
    }
  }, 0);
}
```
- example usage
```shell
...
      // Proxying requires this form vs. callback as last arg.
      return monitorProxy.control(params.name, params.params, function(err, returnParams) {
        onReturn(err, returnParams);
      });
    }
    logId = logId + '.' + probe.probeClass + '.' + params.name;
    log.info(logId + '.request', {params:params.params, probeId:params.probeId});
    return probe.onControl(params.name, params.params, onReturn);
  }

});

/**
* Constructor for a list of Connection objects
*
...
```

#### <a name="apidoc.element.monitor.Probe.prototype.ping_control"></a>[function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>ping_control (params, callback)](#apidoc.element.monitor.Probe.prototype.ping_control)
- description and source-code
```javascript
ping_control = function (params, callback) {
  return callback(null, 'pong');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Probe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>release ()](#apidoc.element.monitor.Probe.prototype.release)
- description and source-code
```javascript
release = function (){
  var t = this;
  log.info('release', t.toJSON());
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```

#### <a name="apidoc.element.monitor.Probe.prototype.set_control"></a>[function <span class="apidocSignatureSpan">monitor.Probe.prototype.</span>set_control (attrs, callback)](#apidoc.element.monitor.Probe.prototype.set_control)
- description and source-code
```javascript
set_control = function (attrs, callback) {
  var t = this,
      writableAttributes = t.get('writableAttributes') || [];

  // Validate the attributes are writable
  if (writableAttributes !== '*') {
    for (var attrName in attrs) {
      if (writableAttributes.indexOf(attrName) < 0) {
        return callback({code:'NOT_WRITABLE', msg: 'Attribute not writable: ' + attrName});
      }
    }
  }

  // Set the data
  var error = null;
  if (!t.set(attrs)) {
    error = {code:'VALIDATION_ERROR', msg:'Data set failed validation'};
    log.warn('set_control', error);
  }
  return callback(error);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.ProcessProbe"></a>[module monitor.ProcessProbe](#apidoc.module.monitor.ProcessProbe)

#### <a name="apidoc.element.monitor.ProcessProbe.ProcessProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>ProcessProbe ()](#apidoc.element.monitor.ProcessProbe.ProcessProbe)
- description and source-code
```javascript
ProcessProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ProcessProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.ProcessProbe.</span>List ()](#apidoc.element.monitor.ProcessProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.ProcessProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.ProcessProbe.</span>extend (params)](#apidoc.element.monitor.ProcessProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.ProcessProbe.prototype"></a>[module monitor.ProcessProbe.prototype](#apidoc.module.monitor.ProcessProbe.prototype)

#### <a name="apidoc.element.monitor.ProcessProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.ProcessProbe.prototype.</span>constructor ()](#apidoc.element.monitor.ProcessProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ProcessProbe.prototype.poll"></a>[function <span class="apidocSignatureSpan">monitor.ProcessProbe.prototype.</span>poll ()](#apidoc.element.monitor.ProcessProbe.prototype.poll)
- description and source-code
```javascript
poll = function () {
  var t = this,
  attrs = _.extend({
    platform: process.platform,
    version: process.version,
    installPrefix: process.installPrefix,
    title: process.title,
    execPath: process.execPath,
    argv: process.argv,
    env: process.env,
    cwd: process.cwd(),
    gid: process.getgid ? process.getgid() : 0,
    uid: process.getuid ? process.getuid() : 0,
    pid: process.pid,
    umask: process.umask(),
    hostname: OS.hostname(),
    type: OS.type(),
    release: OS.release(),
    osUptime: OS.uptime(),
    loadavg: OS.loadavg(),
    freemem: OS.freemem(),
    totalmem: OS.totalmem(),
    cpus: OS.cpus()
  }, process.memoryUsage());
  if (process.uptime) {attrs.uptime = process.uptime();}
  if (process.versions) {attrs.versions = process.versions;}
  if (process.arch) {attrs.arch = process.arch;}
  t.set(attrs);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.RecipeProbe"></a>[module monitor.RecipeProbe](#apidoc.module.monitor.RecipeProbe)

#### <a name="apidoc.element.monitor.RecipeProbe.RecipeProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>RecipeProbe ()](#apidoc.element.monitor.RecipeProbe.RecipeProbe)
- description and source-code
```javascript
RecipeProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.</span>List ()](#apidoc.element.monitor.RecipeProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.RecipeProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.</span>extend (params)](#apidoc.element.monitor.RecipeProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.RecipeProbe.prototype"></a>[module monitor.RecipeProbe.prototype](#apidoc.module.monitor.RecipeProbe.prototype)

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.bringLocal"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>bringLocal (context)](#apidoc.element.monitor.RecipeProbe.prototype.bringLocal)
- description and source-code
```javascript
bringLocal = function (context) {
  var varName,
      localVars = [];
  for (varName in context) {
    localVars.push('var ' + varName + ' = context.' + varName + ';');
  }
  return localVars.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.connectListeners"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>connectListeners (connect)](#apidoc.element.monitor.RecipeProbe.prototype.connectListeners)
- description and source-code
```javascript
connectListeners = function (connect) {
  var t = this,
      triggeredBy = t.get('triggeredBy'),
      onTrigger = t.onTrigger.bind(t);

  // Default to listen on changes to all monitors
  if (!triggeredBy) {
    for (var monitorName in t.monitors) {
      t.monitors[monitorName][connect ? 'on' : 'off']('change', t.onTrigger, t);
    }
    return;
  }

  // Process the elements in triggeredBy
  for (var name in triggeredBy) {
    var value = triggeredBy[name];

    // Construct a new cron job
    if (name === 'cron') {
      if (connect) {
        t.cronJob = new Cron.CronJob(value, onTrigger);
      }
      else {
        if (t.cronJob.initiated) {
          clearInterval(t.CronJob.timer);
        }
        else {
          setTimeout(function(){clearInterval(t.cronJob.timer);}, 1000);
        }
      }
    }

    // Set a polling interval
    else if (name === 'interval') {
      if (connect) {
        t.interval = setInterval(onTrigger, value);
      }
      else {
        clearInterval(t.interval);
        t.interval = null;
      }
    }

    // Must be a monitor name
    else {
      t.monitors[name][connect ? 'on' : 'off'](value, onTrigger);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>constructor ()](#apidoc.element.monitor.RecipeProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.RecipeProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (attributes, options){
  var t = this;

  // Periodic triggers
  t.interval = null;
  t.cronJob = null;

  // Precondition test
  if (_.size(t.get('monitors')) === 0) {
    logger.error('initialize', 'No monitors defined in the recipe');
    return;
  }

  // This is a list of monitors (vs. monitor definitions)
  t.monitors = {};

  // Auto start, calling the callback when started
  if (t.get('autoStart')) {
    options.asyncInit = true;
    t.start_control({}, options.callback);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.onTrigger"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>onTrigger ()](#apidoc.element.monitor.RecipeProbe.prototype.onTrigger)
- description and source-code
```javascript
onTrigger = function () {
  var t = this;
  t.run_control({}, function(error){
    if (error) {
      logger.error('onTrigger', error);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>release ()](#apidoc.element.monitor.RecipeProbe.prototype.release)
- description and source-code
```javascript
release = function () {
  var t = this,
      args = arguments;
  t.stop_control({}, function(){
    Probe.prototype.release.apply(t, args);
  });
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.run"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>run (context)](#apidoc.element.monitor.RecipeProbe.prototype.run)
- description and source-code
```javascript
run = function (context) {
  var t = this,
      script = t.get('script');

  // Run in a VM or exec (if running in a browser)
  if (vm) {
    // Compile the script on first run.  This throws an exception if
    // the script has a problem compiling.
    if (!t.compiledScript) {
      t.compiledScript = vm.createScript(script);
    }

    // Execute the compiled script
    t.compiledScript.runInContext(context, t.name);
  }
  else {
    // Bring all context variables local, then execute the script
    eval(t.bringLocal(context));
    eval(script);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.run_control"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>run_control (params, callback)](#apidoc.element.monitor.RecipeProbe.prototype.run_control)
- description and source-code
```javascript
run_control = function (params, callback) {
  var t = this,
      error = null;
  if (!t.get('started')) {
    error = {code:'NOT_RUNNING', msg:'Cannot run - recipe not started.'};
    logger.warn(error);
    return callback(error);
  }

  // Name the probe
  t.name = t.get('probeName') || t.get('id');

  // Build a context to pass onto the script.  The context contains
  // a console, a logger, and each monitor by name.
  if (!t.context) {
    t.context = vm ? vm.createContext({}) : {};
    t.context.console = console;
    t.context.logger = Monitor.getLogger('Recipe.run.' + t.name);
    for (var monitorName in t.monitors) {
      t.context[monitorName] = t.monitors[monitorName];
    }
  }

  // Run the script
  try {
    t.run(t.context);
  } catch(e) {
    error = "Error running script: " + e.toString();
    logger.error('run_control', error);
  }
  callback(error);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.start_control"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>start_control (params, callback)](#apidoc.element.monitor.RecipeProbe.prototype.start_control)
- description and source-code
```javascript
start_control = function (params, callback) {
  var t = this,
      connectError = false,
      monitors = t.get('monitors');

  if (t.get('started')) {
    var err = {code:'RUNNING', msg:'Cannot start - the recipe is already running.'};
    logger.warn(err);
    return callback(err);
  }

  // Called when a monitor has connected
  var onConnect = function(error) {
    if (connectError) {return;}
    if (error) {
      var err = {code:'CONNECT_ERROR', err: error};
      connectError = true;
      logger.error('start', err);
      return callback(err);
    }
    for (var name1 in t.monitors) {
      if (!t.monitors[name1].isConnected()) {
        return;
      }
    }
    t.set({started:true});
    t.connectListeners(true);
    callback();
  };

  // Connect all monitors
  for (var name2 in monitors) {
    t.monitors[name2] = new Monitor(monitors[name2]);
    t.monitors[name2].connect(onConnect);
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.RecipeProbe.prototype.stop_control"></a>[function <span class="apidocSignatureSpan">monitor.RecipeProbe.prototype.</span>stop_control (params, callback)](#apidoc.element.monitor.RecipeProbe.prototype.stop_control)
- description and source-code
```javascript
stop_control = function (params, callback) {
  var t = this,
      disconnectError = false;

  if (!t.get('started')) {
    var err = {code:'NOT_RUNNING', msg:'The recipe is already stopped.'};
    logger.warn('precondition', err);
    return callback(err);
  }

  // Called when a monitor has disconnected
  var onDisconnect = function(error) {
    if (disconnectError) {return;}
    if (error) {
      var err = {code:'DISONNECT_ERROR', err: error};
      disconnectError = true;
      logger.error('onDisconnect', err);
      return callback(err);
    }
    for (var name1 in t.monitors) {
      if (t.monitors[name1].isConnected()) {
        return;
      }
    }
    t.set({started:false});
    t.compiledScript = null;
    callback();
  };

  // Disconnect all monitors
  t.connectListeners(false);
  t.context = null;
  for (var name2 in t.monitors) {
    t.monitors[name2].disconnect(onDisconnect);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.ReplProbe"></a>[module monitor.ReplProbe](#apidoc.module.monitor.ReplProbe)

#### <a name="apidoc.element.monitor.ReplProbe.ReplProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>ReplProbe ()](#apidoc.element.monitor.ReplProbe.ReplProbe)
- description and source-code
```javascript
ReplProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ReplProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.</span>List ()](#apidoc.element.monitor.ReplProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.ReplProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.</span>extend (params)](#apidoc.element.monitor.ReplProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.ReplProbe.prototype"></a>[module monitor.ReplProbe.prototype](#apidoc.module.monitor.ReplProbe.prototype)

#### <a name="apidoc.element.monitor.ReplProbe.prototype._output"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>_output (str)](#apidoc.element.monitor.ReplProbe.prototype._output)
- description and source-code
```javascript
_output = function (str) {
  var t = this;
  t.set({
    output: str,
    sequence: t.get('sequence') + 1
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ReplProbe.prototype._runShellCmd"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>_runShellCmd (command)](#apidoc.element.monitor.ReplProbe.prototype._runShellCmd)
- description and source-code
```javascript
_runShellCmd = function (command) {
  var t = this;
  t.shellCmd = ChildProcess.exec(command, function(err, stdout, stderr) {
    if (err) {
      var outstr = 'exit';
      if (err.code) {
        outstr += ' (' + err.code + ')';
      }
      if (err.signal) {
        outstr += ' ' + err.signal;
      }
      t._output(outstr);
      return null;
    }
    if (stdout.length) {
      t._output(stdout);
    }
    if (stderr.length) {
      t._output(stderr);
    }
    t.shellCmd = null;
    t._output(CONSOLE_PROMPT);
  });
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ReplProbe.prototype.autocomplete_control"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>autocomplete_control (params, callback)](#apidoc.element.monitor.ReplProbe.prototype.autocomplete_control)
- description and source-code
```javascript
autocomplete_control = function (params, callback) {
  var t = this;
  if (typeof(params) !== 'string' || params.length < 1) {
    callback("Autocomplete paramter must be a nonzero string");
  }

  // Forward to the completion mechanism if it can be completed
  if (params.substr(-1).match(/([0-9])|([a-z])|([A-Z])|([_])/)) {
    t.repl.complete(params, callback);
  } else {
    // Return a no-op autocomplete
    callback(null, [[],'']);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ReplProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>constructor ()](#apidoc.element.monitor.ReplProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ReplProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.ReplProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (attributes, options){
  var t = this;
  Probe.prototype.initialize.apply(t, arguments);

  // Don't send change events before connected
  process.nextTick(function(){
    t.stream = new ReplStream(t);
    if (NEW_REPL) {
      t.repl = require('repl').start({
        prompt: CONSOLE_PROMPT,
        input: t.stream,
        output: t.stream
      });
    } else {
      t.repl = REPL.start(CONSOLE_PROMPT, t.stream);
    }
    t.htmlConsole = new HtmlConsole(t);
    t.shellCmd = null;
    t.repl.context.console = t.htmlConsole;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ReplProbe.prototype.input_control"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>input_control (params, callback)](#apidoc.element.monitor.ReplProbe.prototype.input_control)
- description and source-code
```javascript
input_control = function (params, callback) {
  var t = this;
  if (params === '.break' && t.shellCmd) {
    t.shellCmd.kill();
  }
  if (NEW_REPL) {
    t.stream.emit('data', params + "\n");
  } else {
    t.stream.emit('data', params);
  }
  return callback(null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.ReplProbe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>release ()](#apidoc.element.monitor.ReplProbe.prototype.release)
- description and source-code
```javascript
release = function (){
  var t = this;
  t.stream = null;
  t.repl = null;
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```

#### <a name="apidoc.element.monitor.ReplProbe.prototype.sh_control"></a>[function <span class="apidocSignatureSpan">monitor.ReplProbe.prototype.</span>sh_control (params, callback)](#apidoc.element.monitor.ReplProbe.prototype.sh_control)
- description and source-code
```javascript
sh_control = function (params, callback) {
  var t = this;
  return callback(null, t._runShellCmd(params));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Router"></a>[module monitor.Router](#apidoc.module.monitor.Router)

#### <a name="apidoc.element.monitor.Router.Router"></a>[function <span class="apidocSignatureSpan">monitor.</span>Router ()](#apidoc.element.monitor.Router.Router)
- description and source-code
```javascript
Router = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Router.extend"></a>[function <span class="apidocSignatureSpan">monitor.Router.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Router.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Router.prototype"></a>[module monitor.Router.prototype](#apidoc.module.monitor.Router.prototype)

#### <a name="apidoc.element.monitor.Router.prototype.addConnection"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>addConnection (options)](#apidoc.element.monitor.Router.prototype.addConnection)
- description and source-code
```javascript
addConnection = function (options) {
  var t = this,
      startTime = Date.now();

  // Default the firewall value
  if (_.isUndefined(options.firewall)) {
    options = _.extend({},options, {firewall: t.firewall});
  }

  // Generate a unique ID for the connection
  options.id = Monitor.generateUniqueCollectionId(t.connections);

  var connStr = 'Conn_' + options.id;
  if (options.hostName) {
    connStr += ' - ' + options.hostName + ':' + options.hostPort;
  }
  log.info('addConnection', connStr);

  // Instantiate and add the connection for use, once connected
  var connection = new Connection(options);

  // Add a connect and disconnect function
  var onConnect = function(){
    t.trigger('connection:add', connection);
    log.info('connected', connStr, (Date.now() - startTime) + 'ms');
  };
  var onDisconnect = function(){
    t.removeConnection(connection);
    connection.off('connect', onConnect);
    connection.off('disconnect', onConnect);
    log.info('disconnected', connStr, (Date.now() - startTime) + 'ms');
  };
  connection.on('connect', onConnect);
  connection.on('disconnect', onDisconnect);

  // Add to the connections
  t.connections.add(connection);
  return connection;
}
```
- example usage
```shell
...
*   @param options.socket {io.socket} - Pre-connected socket.io socket to the gateway server.
* @return connection {Connection} - The connection with the gateway server
*/
setGateway: function(options) {
  var t = this;
  options.gateway = false;     // New connection can't be an inbound gateway
  options.firewall = true;     // Gateways are for outbound requests only
  return t.defaultGateway = t.addConnection(options);
},

/**
* Return a stable host name.
*
* @method getHostName
* @protected
...
```

#### <a name="apidoc.element.monitor.Router.prototype.addHostConnections"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>addHostConnections (hostName, callback)](#apidoc.element.monitor.Router.prototype.addHostConnections)
- description and source-code
```javascript
addHostConnections = function (hostName, callback) {
  var t = this,
      errStr = '',
      connectedPorts = [],
      portStart = Config.Monitor.serviceBasePort,
      portEnd = Config.Monitor.serviceBasePort + Config.Monitor.portsToScan - 1;

  // Create an array to hold callbacks for this host
  if (!t.addHostCallbacks[hostName]) {
    t.addHostCallbacks[hostName] = [];
  }

  // Remember this callback and return if we're already adding connections for this host
  if (t.addHostCallbacks[hostName].push(callback) > 1) {
    return;
  }

  // Called when done
  var doneAdding = function(error) {
    t.addHostCallbacks[hostName].forEach(function(cb) {
      cb(error);
    });
    delete t.addHostCallbacks[hostName];
  };

  // Build the list of ports already connected
  t.connections.each(function(connection){
    var host = connection.get('hostName').toLowerCase();
    var port = connection.get('hostPort');
    if (host === hostName && port >= portStart && port <= portEnd) {
      connectedPorts.push(port);
    }
  });

  // Scan non-connected ports
  var portsToScan = Config.Monitor.portsToScan - connectedPorts.length;
  if (portsToScan === 0) {
    errStr = 'All monitor ports in use.  Increase the Config.Monitor.portsToScan configuration';
    log.error('addHostConnections', errStr);
    return doneAdding(errStr);
  }
  var doneScanning = function() {
    var conn = this; // called in the context of the connection
    conn.off('connect disconnect error', doneScanning);
    if (--portsToScan === 0) {
      return doneAdding();
    }
  };
  for (var i = portStart; i <= portEnd; i++) {
    if (connectedPorts.indexOf(i) < 0) {
      var connection = t.addConnection({hostName:hostName, hostPort:i});
      connection.on('connect disconnect error', doneScanning, connection);
    }
  }
}
```
- example usage
```shell
...
      if (t.defaultGateway) {
        connection = t.defaultGateway;
        return connectedCheck(true);
      }

      // See if we can establish new connections with the host
      if (hostName && makeNewConnections) {
        t.addHostConnections(hostName, function(err) {
if (err) {
  log.error('connect.toHost', err);
  return callback(err);
}

// Try finding now that new connections have been made
connection = t.findConnection(hostName, appName, appInstance);
...
```

#### <a name="apidoc.element.monitor.Router.prototype.buildProbeKey"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>buildProbeKey (probeJSON)](#apidoc.element.monitor.Router.prototype.buildProbeKey)
- description and source-code
```javascript
buildProbeKey = function (probeJSON) {
  var probeKey = probeJSON.probeClass,
      initParams = probeJSON.initParams;

  // Allow probes to be externally identified by name
  if (probeJSON.probeName) {
    return probeJSON.probeName;
  }

  if (initParams) {
    _.keys(initParams).sort().forEach(function(key){
      probeKey += ':' + key + '=' + initParams[key];
    });
  }
  return probeKey;
}
```
- example usage
```shell
...
    *     @param monitorJSON.initParams {Object} - Probe initialization parameters.
    * @param callback {Function(error, probeImpl)} - Called when connected
    */
    connectInternal: function(monitorJSON, callback) {

// Build a key for this probe from the probeClass and initParams
var t = this,
    probeKey = t.buildProbeKey(monitorJSON),
    probeName = monitorJSON.probeName,
    probeClass = monitorJSON.probeClass,
    initParams = monitorJSON.initParams,
    probeImpl = null;

var whenDone = function(error) {
...
```

#### <a name="apidoc.element.monitor.Router.prototype.connectExternal"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>connectExternal (monitorJSON, connection, callback)](#apidoc.element.monitor.Router.prototype.connectExternal)
- description and source-code
```javascript
connectExternal = function (monitorJSON, connection, callback) {

  // Build a key for this probe from the probeClass and initParams
  var t = this,
      errStr = '',
      probeKey = t.buildProbeKey(monitorJSON);

  // Get the probe proxy
  var probeId = connection.remoteProbeIdsByKey[probeKey];
  var probeProxy = connection.remoteProbesById[probeId];

  if (!probeProxy) {

    // Connect with the remote probe
    connection.emit('probe:connect', monitorJSON, function(error, probeJSON){
      if (error) {
        errStr = "probe:connect returned an error for probeClass '" + monitorJSON.probeClass +
          "' on " + Monitor.toServerString(monitorJSON);
        return callback({err: error, msg: errStr});
      }
      probeId = probeJSON.id;

      // See if the proxy was created while waiting for return
      probeProxy = connection.remoteProbesById[probeId];
      if (probeProxy) {
        probeProxy.refCount++;
        log.info('connectExternal.connected.existingProxy', {probeId: probeId, refCount: probeProxy.refCount, whileWaiting: true
});
        return callback(null, probeProxy);
      }

      // Create the probe proxy
      probeProxy = new Probe(probeJSON);
      probeProxy.refCount = 1;
      probeProxy.connection = connection;
      connection.remoteProbeIdsByKey[probeKey] = probeId;
      connection.remoteProbesById[probeId] = probeProxy;
      connection.addEvent('probe:change:' + probeId, function(attrs){probeProxy.set(attrs);});
      log.info('connectExternal.connected.newProxy', {probeId: probeId});
      return callback(null, probeProxy);
    });
    return;
  }

  // Probes are released based on reference count
  probeProxy.refCount++;
  log.info('connectExternal.connected.existingProxy', {probeId: probeId, refCount: probeProxy.refCount});
  return callback(null, probeProxy);
}
```
- example usage
```shell
...
      t.on('disconnect', function() {
        t.probeDisconnect({probeId:probeId});
      });
    };

    // Connect internally or externally
    if (connection) {
      router.connectExternal(monitorJSON, connection, onConnect);
    } else {
      router.connectInternal(monitorJSON, onConnect);
    }
  });
},

/**
...
```

#### <a name="apidoc.element.monitor.Router.prototype.connectInternal"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>connectInternal (monitorJSON, callback)](#apidoc.element.monitor.Router.prototype.connectInternal)
- description and source-code
```javascript
connectInternal = function (monitorJSON, callback) {

  // Build a key for this probe from the probeClass and initParams
  var t = this,
      probeKey = t.buildProbeKey(monitorJSON),
      probeName = monitorJSON.probeName,
      probeClass = monitorJSON.probeClass,
      initParams = monitorJSON.initParams,
      probeImpl = null;

  var whenDone = function(error) {

    // Wait one tick before firing the callback.  This simulates a remote
    // connection, making the client callback order consistent, regardless
    // of a local or remote connection.
    setTimeout(function() {

      // Dont connect the probe on error
      if (error) {
        if (probeImpl) {
          delete t.runningProbesByKey[probeKey];
          delete t.runningProbesById[probeImpl.id];
          try {
            // This may fail depending on how many resources were created
            // by the probe before failure.  Ignore errors.
            probeImpl.release();
          } catch (e){}
        }
        return callback(error);
      }

      // Probes are released based on reference count
      probeImpl.refCount++;
      log.info('connectInternal', {probeKey: probeKey, probeId: probeImpl.id});
      callback(null, probeImpl);
    }, 0);
  };

  // Get the probe instance
  probeImpl = t.runningProbesByKey[probeKey];
  if (!probeImpl) {

    // Instantiate the probe
    var ProbeClass = Probe.classes[probeClass];
    if (!ProbeClass) {
      return whenDone({msg:'Probe not available: ' + probeClass});
    }
    var initOptions = {asyncInit: false, callback: whenDone};
    try {
      // Deep copy the init params, because Backbone mutates them.  This
      // is bad if the init params came in from defaults of another object,
      // because those defaults will get mutated.
      var paramCopy = Monitor.deepCopy(initParams);

      // Extend the probe name into the probe if known
      if (probeName) {
        paramCopy.probeName = probeName;
      }

      // Instantiate a new probe
      probeImpl = new ProbeClass(paramCopy, initOptions);
      probeImpl.set({
        id: Monitor.generateUniqueId(),
        writableAttributes: ProbeClass.prototype.writableAttributes || []
      });
      probeImpl.refCount = 0;
      probeImpl.probeKey = probeKey;
      t.runningProbesByKey[probeKey] = probeImpl;
      t.runningProbesById[probeImpl.id] = probeImpl;
    } catch (e) {
      var error = {msg: 'Error instantiating probe ' + probeClass, error: e.message};
      return whenDone(error);
    }

    // Return early if the probe constructor transferred responsibility
    // for calling the callback.
    if (initOptions.asyncInit) {
      return;
    }
  }

  // The probe impl is found, and instantiated if necessary
  whenDone();
}
```
- example usage
```shell
...
      });
    };

    // Connect internally or externally
    if (connection) {
      router.connectExternal(monitorJSON, connection, onConnect);
    } else {
      router.connectInternal(monitorJSON, onConnect);
    }
  });
},

/**
* Process an inbound request to disconnect with a probe
*
...
```

#### <a name="apidoc.element.monitor.Router.prototype.connectMonitor"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>connectMonitor (monitor, callback)](#apidoc.element.monitor.Router.prototype.connectMonitor)
- description and source-code
```javascript
connectMonitor = function (monitor, callback) {

  callback = callback || function(){};
  var t = this,
      monitorJSON = monitor.toMonitorJSON(),
      probeJSON = null,
      probeName = monitorJSON.probeName,
      probeClass = monitorJSON.probeClass,
      startTime = Date.now(),
      monitorStr = probeClass + '.' + monitor.toServerString().replace(/:/g, '.');

  // Class name must be set
  if (!probeClass && !probeName) {
    var errStr = 'probeName or probeClass must be set';
    log.error('connectMonitor', errStr);
    return callback(errStr);
  }

  // Determine the connection (or internal), and listen for change events
  t.determineConnection(monitorJSON, true, function(err, connection) {
    if (err) {return callback(err);}

    // Function to run on connection (internal or external)
    var onConnect = function(error, probe) {
      if (error) {return callback(error);}
      probeJSON = probe.toJSON();
      probeJSON.probeId = probeJSON.id; delete probeJSON.id;
      monitor.probe = probe;

      // Keep the last known probe state for effective updating
      monitor._probeValues = _.clone(probeJSON);

      // Perform the initial set silently.  This assures the initial
      // probe contents are available on the connect event,
      // but doesn't fire a change event before connect.
      monitor.set(probeJSON, {silent:true});

      // Watch the probe for changes.
      monitor.probeChange = function(){
        var changed = probe.changedAttributes();
        if (changed) {
          monitor._probeValues = _.clone(probe.toJSON());
          monitor.set(probe.changedAttributes());
          log.info('probeChange', {probeId: probeJSON.probeId, changed: probe.changedAttributes()});
        }
      };
      probe.on('change', monitor.probeChange);

      // Call the callback.  This calls the original caller, issues
      // the connect event, then fires the initial change event.
      callback(null);
    };

    // Connect internally or externally
    if (connection) {
      t.connectExternal(monitorJSON, connection, onConnect);
    } else {
      t.connectInternal(monitorJSON, onConnect);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Router.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>constructor ()](#apidoc.element.monitor.Router.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Router.prototype.determineConnection"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>determineConnection (monitorJSON, makeNewConnections, callback)](#apidoc.element.monitor.Router.prototype.determineConnection)
- description and source-code
```javascript
determineConnection = function (monitorJSON, makeNewConnections, callback) {
  var t = this,
      connection = null,
      probeName = monitorJSON.probeName,
      probeClass = monitorJSON.probeClass,
      errStr = '',
      hostName = monitorJSON.hostName,
      appName = monitorJSON.appName,
      appInstance = monitorJSON.appInstance,
      thisHostName = t.getHostName().toLowerCase(),
      thisAppName = Config.Monitor.appName  || 'unknown',
      thisAppInstance = typeof process !== 'undefined' ? process.env.NODE_APP_INSTANCE : '1';

  // Return a found connection immediately if it's connected.
  // If connecting, wait for connection to complete.
  // If not connected (and not connecting) re-try the connection.
  var connectedCheck = function(isGateway) {

    // Remove the host/app/instance params if connecting directly.
    if (!isGateway) {
      delete monitorJSON.hostName;
      delete monitorJSON.appName;
      delete monitorJSON.appInstance;
    }

    // Define the connect/error listeners
    var onConnect = function() {
      removeListeners();
      callback(null, connection);
    };
    var onError = function(err) {
      removeListeners();
      log.error('connect.error', err);
      callback({msg: 'connection error', err:err});
    };
    var removeListeners = function() {
      connection.off('connect', onConnect);
      connection.off('error', onError);
    };

    // Wait if the connection is still awaiting connect
    if (connection && connection.connecting) {
      connection.on('connect', onConnect);
      connection.on('error', onError);
      return;
    }

    // Re-try if disconnected
    if (connection && !connection.connected) {
      connection.on('connect', onConnect);
      connection.on('error', onError);
      return connection.connect();
    }

    // Verified connection
    return callback(null, connection);
  };

  // Connect with this process (internally)?
  hostName = hostName ? hostName.toLowerCase() : null;
  var thisHost = (!hostName || hostName === thisHostName);
  var thisApp = (!appName || appName === thisAppName);
  var thisInstance = (!appInstance || appInstance === thisAppInstance);
  if (thisHost && thisApp && thisInstance) {

    // Connect internally if the probe is available
    if (t.runningProbesByKey[probeName] || Probe.classes[probeClass] != null) {
      return callback(null, null);
    }

    // Give named auto-start probes time to start up
    var autoStarts = Monitor.Config.Monitor.autoStart;
    if (probeName && !probeClass && autoStarts.length) {
      var autoStart = Monitor._.find(autoStarts, function(probeDef) {
        return probeDef.probeName === probeName;
      });
      if (autoStart) {
        setTimeout(function() {
          t.determineConnection(monitorJSON, makeNewConnections, callback);
        },10);
        return;
      }
    }

    // No probe with that name in this process.
    // Fallback to the default gateway.
    if (!t.defaultGateway) {
      errStr = 'Probe class "' + probeClass + '" not available in this process';
      log.error('connect.internal', errStr);
      return callback({err:errStr});
    }
    connection = t.defaultGateway;
    return connectedCheck(true);
  }

  // Return if connection is known
  connection = t.findConnection(hostName, appName, appInstance);
  if (connection) {
    return connectedCheck();
  }

  // Prefer the gateway if it exists
  if (t.defaultGateway) {
    connection = t.defaultGateway;
    return connectedCheck(true);
  }

  // See if we can establish new connections with the host
  if (hostName && makeNewConnections) {
    t.addHostConnections(hostName, function(err) {
      if (err) {
        log.error('connect.toHost', err);
        return callback(err);
      }

      // Try finding now that new connections have been made
      connection = t.findConnection(hostName, appName, appInstance);
      if (!connection) {
        errStr = 'No route to host: ' + Monitor.toServerString(monitorJSON);
        log.error('connect.toHost', errStr);
        return callback({err:errStr});
      }

      return connectedCheck(); ...
```
- example usage
```shell
...
      if (firewall) {
        errorText = 'firewalled';
        log.error('probeConnect', errorText, logCtxt);
        return callback(errorText);
      }

      // Determine the connection to use (or internal)
      router.determineConnection(monitorJSON, gateway, function(err, connection) {
        if (err) {return callback(err);}
        if (connection && !gateway) {return callback('Not a gateway');}

        // Function to run upon connection (internal or external)
        var onConnect = function(error, probe) {

if (error) {
...
```

#### <a name="apidoc.element.monitor.Router.prototype.disconnectExternal"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>disconnectExternal (connection, probeId, callback)](#apidoc.element.monitor.Router.prototype.disconnectExternal)
- description and source-code
```javascript
disconnectExternal = function (connection, probeId, callback) {
  var t = this, proxy = connection.remoteProbesById[probeId];
  if (!proxy) {return callback('Probe not running');}
  if (--proxy.refCount === 0) {
    // Release probe resources
    proxy.release();
    proxy.connection = null;
    delete connection.remoteProbesById[probeId];
    delete connection.remoteProbeIdsByKey[proxy.probeKey];
    connection.removeEvent('probe:change:' + probeId);
    return connection.emit('probe:disconnect', {probeId:probeId}, function(error){
      return callback(error);
    });
  }
  callback(null);
}
```
- example usage
```shell
...
    log.info(t.logId + 'probeDisconnected', logCtxt);
    stat.time(t.logId + 'probeDisconnected', duration);
    return callback(null);
  };

  // Disconnect from an internal or external probe
  if (probe && probe.connection) {
    router.disconnectExternal(probe.connection, probeId, onDisconnect);
  } else {
    router.disconnectInternal(probeId, onDisconnect);
  }
},

/**
* Process an inbound control request to a probe
...
```

#### <a name="apidoc.element.monitor.Router.prototype.disconnectInternal"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>disconnectInternal (probeId, callback)](#apidoc.element.monitor.Router.prototype.disconnectInternal)
- description and source-code
```javascript
disconnectInternal = function (probeId, callback) {
  var t = this, probeImpl = t.runningProbesById[probeId];
  if (!probeImpl) {return callback('Probe not running');}
  if (--probeImpl.refCount === 0) {

    // Release probe resources & internal references if still no references after a while
    setTimeout(function() {
      if (probeImpl.refCount === 0) {
        try {
          probeImpl.release();
        } catch (e){}
        delete t.runningProbesByKey[probeImpl.probeKey];
        delete t.runningProbesById[probeId];
      }
    }, PROBE_TIMEOUT_MS);
  }
  callback(null, probeImpl);
}
```
- example usage
```shell
...
    return callback(null);
  };

  // Disconnect from an internal or external probe
  if (probe && probe.connection) {
    router.disconnectExternal(probe.connection, probeId, onDisconnect);
  } else {
    router.disconnectInternal(probeId, onDisconnect);
  }
},

/**
* Process an inbound control request to a probe
*
* @method probeControl
...
```

#### <a name="apidoc.element.monitor.Router.prototype.disconnectMonitor"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>disconnectMonitor (monitor, reason, callback)](#apidoc.element.monitor.Router.prototype.disconnectMonitor)
- description and source-code
```javascript
disconnectMonitor = function (monitor, reason, callback) {
  callback = callback || function(){};
  var t = this, probe = monitor.probe, probeId = monitor.get('probeId');

  // The monitor must be connected
  if (!probe) {return callback('Monitor must be connected');}

  // Called upon disconnect (internal or external)
  var onDisconnect = function(error) {
    if (error) {
      return callback(error);
    }
    probe.off('change', monitor.probeChange);
    monitor.set({probeId:null});
    monitor.probe = monitor.probeChange = null;
    return callback(null, reason);
  };

  // Disconnect from an internal or external probe
  if (probe.connection) {
    t.disconnectExternal(probe.connection, probeId, onDisconnect);
  } else {
    t.disconnectInternal(probeId, onDisconnect);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Router.prototype.findConnection"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>findConnection (hostName, appName, appInstance)](#apidoc.element.monitor.Router.prototype.findConnection)
- description and source-code
```javascript
findConnection = function (hostName, appName, appInstance) {
  var t = this, thisInstance = 0;
  return t.connections.find(function(conn) {

    // Host or app matches if not specified or if specified and equal
    var matchesHost = !hostName || conn.isThisHost(hostName);
    var matchesApp = !appName || appName === conn.get('remoteAppName');
    var matchesInstance = !appInstance || appInstance === conn.get('remoteAppInstance');
    var remoteFirewall = conn.get('remoteFirewall');

    // This is a match if host + app + instance matches, and it's not firewalled
    return (!remoteFirewall && matchesHost && matchesApp && matchesInstance);
  });
}
```
- example usage
```shell
...
    return callback({err:errStr});
  }
  connection = t.defaultGateway;
  return connectedCheck(true);
}

// Return if connection is known
connection = t.findConnection(hostName, appName, appInstance);
if (connection) {
  return connectedCheck();
}

// Prefer the gateway if it exists
if (t.defaultGateway) {
  connection = t.defaultGateway;
...
```

#### <a name="apidoc.element.monitor.Router.prototype.findConnections"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>findConnections (hostName, appName)](#apidoc.element.monitor.Router.prototype.findConnections)
- description and source-code
```javascript
findConnections = function (hostName, appName) {
  var t = this;
  return t.connections.filter(function(conn) {

    // Host or app matches if not specified or if specified and equal
    var matchesHost = !hostName || conn.isThisHost(hostName);
    var matchesApp = !appName || appName === conn.get('remoteAppName');
    var remoteFirewall = conn.get('remoteFirewall');

    // This is a match if host + app matches, and it's not firewalled
    return (!remoteFirewall && matchesHost && matchesApp);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Router.prototype.getHostName"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>getHostName ()](#apidoc.element.monitor.Router.prototype.getHostName)
- description and source-code
```javascript
getHostName = function () {
  var localStorage = root.localStorage;
  if (!hostName) {
    if (localStorage) {hostName = localStorage.hostName;}
    hostName = hostName || Monitor.generateUniqueId();
    if (localStorage) {localStorage.hostName = hostName;}
  }
  return hostName;
}
```
- example usage
```shell
...
var pid = typeof process === 'undefined' ? 1 : process.pid;

// Determine the app instance
var appInstance = '' + (typeof process === 'undefined' ? pid : process.env.NODE_APP_INSTANCE || pid);

// Exchange connection information
socket.emit('connection:info', {
  hostName:Monitor.getRouter().getHostName(),
  appName:Config.Monitor.appName,
  appInstance: appInstance,
  pid: pid,
  probeClasses: _.keys(Probe.classes),
  gateway:t.get('gateway'),
  firewall:t.get('firewall')
});
...
```

#### <a name="apidoc.element.monitor.Router.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>initialize ()](#apidoc.element.monitor.Router.prototype.initialize)
- description and source-code
```javascript
initialize = function () {
  var t = this;
  t.defaultGateway = null;
  t.firewall = false;
  t.connections = new Connection.List();
  t.runningProbesByKey = {}; // key=probeKey, data=probeImpl
  t.runningProbesById = {};  // key=probeId, data=probeImpl
  t.addHostCallbacks = {};  // key=hostName, data=[callbacks]
  log.info('init', 'Router initialized');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Router.prototype.removeConnection"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>removeConnection (connection)](#apidoc.element.monitor.Router.prototype.removeConnection)
- description and source-code
```javascript
removeConnection = function (connection) {
  var t = this;
  log.info('removeConnection', 'Conn_' + connection.id);
  connection.disconnect('connection_removed');
  t.connections.remove(connection);
  t.trigger('connection:remove', connection);
}
```
- example usage
```shell
...

// Add a connect and disconnect function
var onConnect = function(){
  t.trigger('connection:add', connection);
  log.info('connected', connStr, (Date.now() - startTime) + 'ms');
};
var onDisconnect = function(){
  t.removeConnection(connection);
  connection.off('connect', onConnect);
  connection.off('disconnect', onConnect);
  log.info('disconnected', connStr, (Date.now() - startTime) + 'ms');
};
connection.on('connect', onConnect);
connection.on('disconnect', onDisconnect);
...
```

#### <a name="apidoc.element.monitor.Router.prototype.setFirewall"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>setFirewall (firewall)](#apidoc.element.monitor.Router.prototype.setFirewall)
- description and source-code
```javascript
setFirewall = function (firewall) {
  var t = Monitor.getRouter(); // This is a static method
  t.firewall = firewall;
  log.info('setFirewall', firewall);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Router.prototype.setGateway"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>setGateway (options)](#apidoc.element.monitor.Router.prototype.setGateway)
- description and source-code
```javascript
setGateway = function (options) {
  var t = this;
  options.gateway = false;     // New connection can't be an inbound gateway
  options.firewall = true;     // Gateways are for outbound requests only
  return t.defaultGateway = t.addConnection(options);
}
```
- example usage
```shell
...
* @extends Backbone.Model
* @constructor
* @param model - Initial data model.  Can be a JS object or another Model.
*   @param [model.hostName] {String} The host name to connect with. Used if url isn't present.
*   @param [model.hostPort] {Number} The host port to connect using. Used if url isn't present.
*   @param [model.url] {String} The URL used to connect. Built if hostName is supplied.
*   @param [model.socket] {io.socket} Use this pre-connected socket instead of creating a new one.
*   @param [model.gateway=false] {Boolean} Allow this connection to use me as a gateway?  See <code><a href="Router.html#method_setGateway
">Router.setGateway()</a></code>
*   @param [model.firewall=false] {Boolean} Firewall inbound probe requests on this connection?
*   @param [model.remoteHostName] {String READONLY} Host name given by the remote server.
*   @param [model.remoteAppName] {String READONLY} App name given by the remote server.
*   @param [model.remoteAppInstance] {Integer READONLY} The remote application instance ID running on the host.
*   @param [model.remotePID] {String READONLY} Remote process ID.
*   @param [model.remoteProbeClasses] {Array of String READONLY} Array of probe classes available to the remote server.
*   @param [model.remoteGateway] {Boolean READONLY} Can the remote process act as a gateway?
...
```

#### <a name="apidoc.element.monitor.Router.prototype.setHostName"></a>[function <span class="apidocSignatureSpan">monitor.Router.prototype.</span>setHostName (name)](#apidoc.element.monitor.Router.prototype.setHostName)
- description and source-code
```javascript
setHostName = function (name) {
  hostName = name;
  log.info('setHostName', name);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Server"></a>[module monitor.Server](#apidoc.module.monitor.Server)

#### <a name="apidoc.element.monitor.Server.Server"></a>[function <span class="apidocSignatureSpan">monitor.</span>Server ()](#apidoc.element.monitor.Server.Server)
- description and source-code
```javascript
Server = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
* due to a firewall or browser restriction, the monitor will attempt the
* connection to the probe through the gateway server.
*
* The server specified in this method must have been started as a gateway
* like this:
*
*     // Start a monitor server and act as a gateway
*     var server = new Monitor.Server({gateway:true});
*
* @method setGateway
* @param options {Object} - Connection parameters
*   @param options.hostName {String} - Name of the gateway host
*   @param options.hostPort {Integer} - Port number to connect with
*   @param options.url {String} - The URL used to connect (created, or used if supplied)
*   @param options.socket {io.socket} - Pre-connected socket.io socket to the gateway server.
...
```

#### <a name="apidoc.element.monitor.Server.List"></a>[function <span class="apidocSignatureSpan">monitor.Server.</span>List ()](#apidoc.element.monitor.Server.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.Server.extend"></a>[function <span class="apidocSignatureSpan">monitor.Server.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Server.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Server.List"></a>[module monitor.Server.List](#apidoc.module.monitor.Server.List)

#### <a name="apidoc.element.monitor.Server.List.List"></a>[function <span class="apidocSignatureSpan">monitor.Server.</span>List ()](#apidoc.element.monitor.Server.List.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.Server.List.extend"></a>[function <span class="apidocSignatureSpan">monitor.Server.List.</span>extend (protoProps, staticProps)](#apidoc.element.monitor.Server.List.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent's constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function.
  var Surrogate = function(){ this.constructor = child; };
  Surrogate.prototype = parent.prototype;
  child.prototype = new Surrogate;

  // Add prototype properties (instance properties) to the subclass,
  // if supplied.
  if (protoProps) _.extend(child.prototype, protoProps);

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.Server.List.prototype"></a>[module monitor.Server.List.prototype](#apidoc.module.monitor.Server.List.prototype)

#### <a name="apidoc.element.monitor.Server.List.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.Server.List.prototype.</span>constructor ()](#apidoc.element.monitor.Server.List.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Server.List.prototype.model"></a>[function <span class="apidocSignatureSpan">monitor.Server.List.prototype.</span>model ()](#apidoc.element.monitor.Server.List.prototype.model)
- description and source-code
```javascript
model = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Server.prototype"></a>[module monitor.Server.prototype](#apidoc.module.monitor.Server.prototype)

#### <a name="apidoc.element.monitor.Server.prototype.bindEvents"></a>[function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>bindEvents (callback)](#apidoc.element.monitor.Server.prototype.bindEvents)
- description and source-code
```javascript
bindEvents = function (callback) {

  // Detect server errors
  var t = this, server = t.get('server');
  server.on('clientError', function(err){
    log.error('bindEvents', 'clientError detected on server', err);
    t.trigger('error', err);
  });
  server.on('close', function(err){
    server.hasEmittedClose = true;
    log.info('bindEvents.serverClose', 'Server has closed', err);
    t.stop();
  });

  // Start up the socket.io server.
  var socketIoParams = {
    log: false
  };
  t.socketServer = SocketIO.listen(server, socketIoParams);
  t.socketServer.sockets.on('connection', function (socket) {
    var connection = Monitor.getRouter().addConnection({
      socket: socket, gateway: t.get('gateway')
    });
    t.connections.add(connection);
    var onDisconnect = function(reason) {
      t.connections.remove(connection);
      Monitor.getRouter().removeConnection(connection);
      connection.off('disconnect', onDisconnect);
      log.info('client.disconnect', 'Disconnected client socket');
    };
    connection.on('disconnect', onDisconnect);
    log.info('client.connect', 'Connected client socket');
  });

  // Notify that we've started
  t.isListening = true;
  if (callback) {callback(null);}
  t.trigger('start');
}
```
- example usage
```shell
...
error = {err:'connect:failure', msg: 'no ports available'};
log.error('start', error);
return callback(error);
      }

      // Bind to an existing server, or create a new server
      if (server) {
t.bindEvents(callback);
      } else {
server = Http.createServer();

// Try next port if a server is listening on this port
server.on('error', function(err) {
  if (err.code === 'EADDRINUSE') {
    // Error if the requested port is in use
...
```

#### <a name="apidoc.element.monitor.Server.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>constructor ()](#apidoc.element.monitor.Server.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Server.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>initialize (params)](#apidoc.element.monitor.Server.prototype.initialize)
- description and source-code
```javascript
initialize = function (params) {
  var t = this;
  t.isListening = false;
  t.connections = new Connection.List();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Server.prototype.start"></a>[function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>start (options, callback)](#apidoc.element.monitor.Server.prototype.start)
- description and source-code
```javascript
start = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = null;
  }
  options = options || {};
  callback = callback || function(){};
  var t = this, server = t.get('server'), error,
      startTime = Date.now(),
      port = options.port || Config.Monitor.serviceBasePort,
      attempt = options.attempt || 1,
      allowExternalConnections = Config.Monitor.allowExternalConnections;

  // Recursion detection.  Only scan for so many ports
  if (attempt > Config.Monitor.portsToScan) {
    error = {err:'connect:failure', msg: 'no ports available'};
    log.error('start', error);
    return callback(error);
  }

  // Bind to an existing server, or create a new server
  if (server) {
    t.bindEvents(callback);
  } else {
    server = Http.createServer();

    // Try next port if a server is listening on this port
    server.on('error', function(err) {
      if (err.code === 'EADDRINUSE') {
        // Error if the requested port is in use
        if (t.get('port')) {
          log.error('portInUse',{host:host, port:port});
          return callback({err:'portInUse'});
        }
        // Try the next port
        log.info('portInUse',{host:host, port:port});
        return t.start({port:port + 1, attempt:attempt + 1}, callback);
      }
      // Unknown error
      callback(err);
    });

    // Allow connections from INADDR_ANY or LOCALHOST only
    var host = allowExternalConnections ? '0.0.0.0' : '127.0.0.1';

    // Start listening, callback on success
    server.listen(port, host, function(){

      // Set a default NODE_APP_INSTANCE based on the available server port
      if (!process.env.NODE_APP_INSTANCE)  {
        process.env.NODE_APP_INSTANCE = '' + (port - Config.Monitor.serviceBasePort + 1);
      }

      // Record the server & port, and bind incoming events
      t.set({server: server, port: port});
      t.bindEvents(callback);
      log.info('listening', {
        appName: Config.Monitor.appName,
        NODE_APP_INSTANCE: process.env.NODE_APP_INSTANCE,
        listeningOn: host,
        port: port
      });
    });
  }
}
```
- example usage
```shell
...

Run the following from your app server directory

    $ npm install monitor

Then place the following line in your application bootstrap, and restart your server

    require('monitor').start();

Monitoring your app with a REPL console
---------------------------------------

Ad-hoc monitoring can be done from a REPL console.

Start up the REPL, and get the Monitor class.  Feel free to copy/paste these lines into your console:
...
```

#### <a name="apidoc.element.monitor.Server.prototype.stop"></a>[function <span class="apidocSignatureSpan">monitor.Server.prototype.</span>stop (callback)](#apidoc.element.monitor.Server.prototype.stop)
- description and source-code
```javascript
stop = function (callback) {
  var t = this, server = t.get('server'), router = Monitor.getRouter();
  callback = callback || function(){};

  // Call the callback, but don't stop more than once.
  if (!t.isListening) {
    return callback();
  }

  // Release resources
  t.connections.each(router.removeConnection, router);
  t.connections.reset();

  // Shut down the server
  t.isListening = false;
  server.close();

  // Send notices
  t.trigger('stop');
  return callback();
}
```
- example usage
```shell
...
server.on('clientError', function(err){
  log.error('bindEvents', 'clientError detected on server', err);
  t.trigger('error', err);
});
server.on('close', function(err){
  server.hasEmittedClose = true;
  log.info('bindEvents.serverClose', 'Server has closed', err);
  t.stop();
});

// Start up the socket.io server.
var socketIoParams = {
  log: false
};
t.socketServer = SocketIO.listen(server, socketIoParams);
...
```



# <a name="apidoc.module.monitor.Stat"></a>[module monitor.Stat](#apidoc.module.monitor.Stat)

#### <a name="apidoc.element.monitor.Stat.Stat"></a>[function <span class="apidocSignatureSpan">monitor.</span>Stat (module)](#apidoc.element.monitor.Stat.Stat)
- description and source-code
```javascript
Stat = function (module) {
  var t = this;
  t.module = module;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat._buildRegex"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>_buildRegex (str)](#apidoc.element.monitor.Stat._buildRegex)
- description and source-code
```javascript
_buildRegex = function (str) {
  var regexStr = '',
      modifier = '',
      lastIdx = str.length - 1,
      inSquiggly = false;

  // Javascript regular expressions
  if (/^\/[^\/]*\/i*$/.test(str)) {
    if (/i$/.test(str)) {
      modifier = 'i';
      str = str.replace(/i$/,'');
    }
    regexStr = '^' + str.replace(/^\//,'').replace(/\/$/,'') + '$';
  }

  // Process character by character
  else {
    for (var i = 0, l = str.length; i < l; i++) {
      var c = str.substr(i,1);
      switch (c) {
        case '.':
          c = '\\.';
          break;
        case '*':
          c = (i === lastIdx ? '.*' : '[^\\.]*');
          break;
        case '{':
          c = '(';
          inSquiggly = true;
          break;
        case '}':
          c = ')';
          inSquiggly = false;
          break;
        case ',':
          if (inSquiggly) {
            c = '|';
          }
          break;
      }
      regexStr += c;
    }

    // Force it to match the full string
    regexStr = '^' + regexStr + '$';
  }

  // Now build the regex.  This throws an exception if poorly formed.
  return new RegExp(regexStr, modifier);
}
```
- example usage
```shell
...
  if (!fullName) {
    fullName = module + '.' + name;
  }

  // Get the regex associated with the name
  var regex = Stat.eventRegex[eventName];
  if (!regex) {
    regex = Stat.eventRegex[eventName] = Stat._buildRegex(eventName);
  }

  // Test the name with the regex, and emit if it matches
  if (regex.test(fullName)) {
    Stat.emit(eventName, module, name, value, type);
  }
}
...
```

#### <a name="apidoc.element.monitor.Stat._emit"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>_emit (module, name, value, type)](#apidoc.element.monitor.Stat._emit)
- description and source-code
```javascript
_emit = function (module, name, value, type) {
  var eventName,
      fullName;

  // Prevent stat recursion. This has the effect of disabling all stats
  // for stat handlers (and their downstream effect), but is necessary to
  // prevent infinite recursion.  If it's desired to stat the output of
  // stat handlers, then delay that processing until nextTick.
  if (emittingNow) {
    return;
  }
  emittingNow = true;

  // Test the name against all registered events
  for (eventName in Stat._events) {

    // Build the full name only if someone is listening
    if (!fullName) {
      fullName = module + '.' + name;
    }

    // Get the regex associated with the name
    var regex = Stat.eventRegex[eventName];
    if (!regex) {
      regex = Stat.eventRegex[eventName] = Stat._buildRegex(eventName);
    }

    // Test the name with the regex, and emit if it matches
    if (regex.test(fullName)) {
      Stat.emit(eventName, module, name, value, type);
    }
  }

  // Turn off recursion prevention
  emittingNow = false;
}
```
- example usage
```shell
...
*
* @method increment
* @param name {String} Dot.separated name of the counter to increment
* @param [value=1] {Number} Amount to increment the counter by.
*/
proto.increment = function(name, value){
  value = _.isNumber(value) ? value : 1;
  Stat._emit(this.module, name, value, 'c');
};

/**
* Decrement a counter by a specified value
*
* Assuming someone is listening to this stat, this is an instruction for that
* listener to subtract the specified value (usually 1) to their prior value for this stat.
...
```

#### <a name="apidoc.element.monitor.Stat.addListener"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>addListener (type, listener)](#apidoc.element.monitor.Stat.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.emit"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>emit (type)](#apidoc.element.monitor.Stat.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
...
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
* Disconnect from the remote process
*
* This can be called from the underlying transport if it detects a disconnect,
* or it can be manually called to force a disconnect.
...
```

#### <a name="apidoc.element.monitor.Stat.eventNames"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>eventNames ()](#apidoc.element.monitor.Stat.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.getMaxListeners"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>getMaxListeners ()](#apidoc.element.monitor.Stat.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.listenerCount"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>listenerCount (type)](#apidoc.element.monitor.Stat.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.listeners"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>listeners (type)](#apidoc.element.monitor.Stat.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.on"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>on (type, listener)](#apidoc.element.monitor.Stat.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:

    > processMonitor.on('change', function() {
    ... console.log(processMonitor.get('freemem'));
    ... });

Monitoring your app with a custom script
----------------------------------------

Using Node.js as a scripting language, you can write custom monitors that do anything Node.js can do.  Here's an example that prints
 to the console when free memory falls below a threshold.
...
```

#### <a name="apidoc.element.monitor.Stat.once"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>once (type, listener)](#apidoc.element.monitor.Stat.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.prependListener"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>prependListener (type, listener)](#apidoc.element.monitor.Stat.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.prependOnceListener"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>prependOnceListener (type, listener)](#apidoc.element.monitor.Stat.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.removeAllListeners"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>removeAllListeners (type)](#apidoc.element.monitor.Stat.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.removeListener"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>removeListener (type, listener)](#apidoc.element.monitor.Stat.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
...
  return t;
},

// Remove the specified event from the socket
removeEvent: function(eventName) {
  var t = this, socket = t.get('socket');
  if (t.socketEvents && t.socketEvents[eventName]) {
    socket.removeListener(eventName, t.socketEvents[eventName]);
    delete t.socketEvents[eventName];
  }
  return t;
},

// Remove all events bound to the socket
removeAllEvents: function() {
...
```

#### <a name="apidoc.element.monitor.Stat.setMaxListeners"></a>[function <span class="apidocSignatureSpan">monitor.Stat.</span>setMaxListeners (n)](#apidoc.element.monitor.Stat.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.Stat.prototype"></a>[module monitor.Stat.prototype](#apidoc.module.monitor.Stat.prototype)

#### <a name="apidoc.element.monitor.Stat.prototype.decrement"></a>[function <span class="apidocSignatureSpan">monitor.Stat.prototype.</span>decrement (name, value)](#apidoc.element.monitor.Stat.prototype.decrement)
- description and source-code
```javascript
decrement = function (name, value){
  value = _.isNumber(value) ? value : 1;
  Stat._emit(this.module, name, value * -1, 'c');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.Stat.prototype.gauge"></a>[function <span class="apidocSignatureSpan">monitor.Stat.prototype.</span>gauge (name, value)](#apidoc.element.monitor.Stat.prototype.gauge)
- description and source-code
```javascript
gauge = function (name, value){
  Stat._emit(this.module, name, value, 'g');
}
```
- example usage
```shell
...
proto.gauge = function(name, value){
  Stat._emit(this.module, name, value, 'g');
};

/**
* Record the specified duration (in milliseconds) for the stat
*
* This is like Stat.gauge() in that it is a client-side setting of a
* specified value.  The difference is the scale of the value is specified
* as milliseconds.
*
* This may be one of the most widely used stat methods.  It can (should?) be
* used upon callback from asynchronous methods.
*
* Pattern:
...
```

#### <a name="apidoc.element.monitor.Stat.prototype.increment"></a>[function <span class="apidocSignatureSpan">monitor.Stat.prototype.</span>increment (name, value)](#apidoc.element.monitor.Stat.prototype.increment)
- description and source-code
```javascript
increment = function (name, value){
  value = _.isNumber(value) ? value : 1;
  Stat._emit(this.module, name, value, 'c');
}
```
- example usage
```shell
...
*
* As a collector, it's a place to send application stats as they're discovered.
*
* Example for incrementing a stat in your application:
*
*     var stat = require('monitor').getStatLogger('myModule');
*     ...
*     stat.increment('requests.inbound');
*
* The above is a request to increment the '''myModule.requests.inbound''' stat.
* It peforms work only if someone is listening for that event.
*
* Stat Emitter
* -------------
* As an emitter, Stat is a place to gather stats as they're collected.
...
```

#### <a name="apidoc.element.monitor.Stat.prototype.time"></a>[function <span class="apidocSignatureSpan">monitor.Stat.prototype.</span>time (name, duration)](#apidoc.element.monitor.Stat.prototype.time)
- description and source-code
```javascript
time = function (name, duration){
  Stat._emit(this.module, name, duration, 'ms');
}
```
- example usage
```shell
...
  }
};
probe.connectTime = Date.now();
var duration = probe.connectTime - startTime;
logCtxt.duration = duration;
logCtxt.refCount = probe.refCount;
log.info(t.logId + 'probeConnected', logCtxt);
stat.time(t.logId + 'probeConnected', duration);
callback(null, probe.toJSON());
probe.on('change', monitorProxy.probeChange);

// Disconnect the probe on connection disconnect
t.on('disconnect', function() {
  t.probeDisconnect({probeId:probeId});
});
...
```



# <a name="apidoc.module.monitor.StatProbe"></a>[module monitor.StatProbe](#apidoc.module.monitor.StatProbe)

#### <a name="apidoc.element.monitor.StatProbe.StatProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>StatProbe ()](#apidoc.element.monitor.StatProbe.StatProbe)
- description and source-code
```javascript
StatProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.StatProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.StatProbe.</span>List ()](#apidoc.element.monitor.StatProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.StatProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.StatProbe.</span>extend (params)](#apidoc.element.monitor.StatProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.StatProbe.prototype"></a>[module monitor.StatProbe.prototype](#apidoc.module.monitor.StatProbe.prototype)

#### <a name="apidoc.element.monitor.StatProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.StatProbe.prototype.</span>constructor ()](#apidoc.element.monitor.StatProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.StatProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.StatProbe.prototype.</span>initialize ()](#apidoc.element.monitor.StatProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (){
  var t = this;

  // Call parent constructor
  StreamProbe.prototype.initialize.apply(t, arguments);

  // The watcher just forwards all args to queueItem as an array
  t.watcher = function() {
    // Add timestamp as the first element
    var logElems = _.toArray(arguments);
    logElems.splice(0,0,JSON.stringify(new Date()).substr(1,24));
    t.queueItem.call(t, logElems);
  };
  Stat.on(t.get('pattern'), t.watcher);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.StatProbe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.StatProbe.prototype.</span>release ()](#apidoc.element.monitor.StatProbe.prototype.release)
- description and source-code
```javascript
release = function () {
  var t = this;
  Stat.off(t.get('pattern'), t.watcher);
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```



# <a name="apidoc.module.monitor.StreamProbe"></a>[module monitor.StreamProbe](#apidoc.module.monitor.StreamProbe)

#### <a name="apidoc.element.monitor.StreamProbe.StreamProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>StreamProbe ()](#apidoc.element.monitor.StreamProbe.StreamProbe)
- description and source-code
```javascript
StreamProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.StreamProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.StreamProbe.</span>List ()](#apidoc.element.monitor.StreamProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.StreamProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.StreamProbe.</span>extend (params)](#apidoc.element.monitor.StreamProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.StreamProbe.prototype"></a>[module monitor.StreamProbe.prototype](#apidoc.module.monitor.StreamProbe.prototype)

#### <a name="apidoc.element.monitor.StreamProbe.prototype._send"></a>[function <span class="apidocSignatureSpan">monitor.StreamProbe.prototype.</span>_send ()](#apidoc.element.monitor.StreamProbe.prototype._send)
- description and source-code
```javascript
_send = function () {
  var t = this,
      now = Date.now();

  // This kicks off the send
  t.lastSendTime = now;
  t.set({
    bundle: t.queue,
    sequence: t.get('sequence') + 1
  });

  // Reset
  t.queue = [];
  if (t.timer) {
    clearTimeout(t.timer);
    t.timer = null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.StreamProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.StreamProbe.prototype.</span>constructor ()](#apidoc.element.monitor.StreamProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.StreamProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.StreamProbe.prototype.</span>initialize ()](#apidoc.element.monitor.StreamProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (){
  var t = this;

  // Initialize parent
  Probe.prototype.initialize.apply(t, arguments);

  // Moving the interval into an instance variable for performance
  t.interval = t.get('interval');

  // Set up for the first bundle
  t.queue = [];
  t.timer = null;
  t.lastSendTime = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.StreamProbe.prototype.queueItem"></a>[function <span class="apidocSignatureSpan">monitor.StreamProbe.prototype.</span>queueItem (item)](#apidoc.element.monitor.StreamProbe.prototype.queueItem)
- description and source-code
```javascript
queueItem = function (item) {
  var t = this,
      now = Date.now(),
      msSinceLastSend = now - t.lastSendTime;

  // Queue the item
  t.queue.push(item);

  // Send the bundle?
  if (msSinceLastSend > t.interval) {
    // It's been a while since the last send.  Send it now.
    t._send();
  }
  else {
    // Start the timer if it's not already running
    if (!t.timer) {
      t.timer = setTimeout(function(){
        t._send();
      }, t.interval - msSinceLastSend);
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.SyncProbe"></a>[module monitor.SyncProbe](#apidoc.module.monitor.SyncProbe)

#### <a name="apidoc.element.monitor.SyncProbe.SyncProbe"></a>[function <span class="apidocSignatureSpan">monitor.</span>SyncProbe ()](#apidoc.element.monitor.SyncProbe.SyncProbe)
- description and source-code
```javascript
SyncProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.</span>FileSyncProbe ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe)
- description and source-code
```javascript
FileSyncProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.</span>List ()](#apidoc.element.monitor.SyncProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.SyncProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.</span>extend (params)](#apidoc.element.monitor.SyncProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```



# <a name="apidoc.module.monitor.SyncProbe.FileSyncProbe"></a>[module monitor.SyncProbe.FileSyncProbe](#apidoc.module.monitor.SyncProbe.FileSyncProbe)

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.FileSyncProbe"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.</span>FileSyncProbe ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.FileSyncProbe)
- description and source-code
```javascript
FileSyncProbe = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.List"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>List ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.List)
- description and source-code
```javascript
List = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
...
  }

});

/**
* Constructor for a list of Connection objects
*
*     var myList = new Connection.List(initialElements);
*
* @static
* @method List
* @param [items] {Array} Initial list items.  These can be raw JS objects or Connection data model objects.
* @return {Backbone.Collection} Collection of Connection data model objects
*/
Connection.List = Backbone.Collection.extend({model: Connection});
...
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.extend"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>extend (params)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.extend)
- description and source-code
```javascript
extend = function (params) {
  var t = this, probeClass = Backbone.Model.extend.apply(t, arguments);
  if (params.probeClass) {Probe.classes[params.probeClass] = probeClass;}
  return probeClass;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.getRootPath"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>getRootPath ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.getRootPath)
- description and source-code
```javascript
getRootPath = function () {
  return ROOT_PATH;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.setRootPath"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.</span>setRootPath (rootPath)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.setRootPath)
- description and source-code
```javascript
setRootPath = function (rootPath) {
  var normalized = Path.normalize(rootPath);
  if (ROOT_PATH && ROOT_PATH !== normalized) {
    throw new Error('Cannot change the File probe root path once set.');
  }
  ROOT_PATH = normalized;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.SyncProbe.FileSyncProbe.prototype"></a>[module monitor.SyncProbe.FileSyncProbe.prototype](#apidoc.module.monitor.SyncProbe.FileSyncProbe.prototype)

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>constructor ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.create_control"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>create_control (args, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.create_control)
- description and source-code
```javascript
create_control = function (args, callback) {
  // Make sure the ID exists
  var t = this, model = args.model;
  if (!model || !model.id) {
    return callback({msg:'SyncProbe create - Data model with ID not present'});
  }

  // Make sure the file doesn't already exist
  t.getFullPath(model.id, function(error, response) {
    if (error) {
      return callback(error);
    }

    if (response.stats) {
      return callback({msg:'Document with this ID already exists'});
    }

    // Forward to the update control
    t.update_control(args, callback);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.delete_control"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>delete_control (args, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.delete_control)
- description and source-code
```javascript
delete_control = function (args, callback) {
  // Make sure the ID exists
  var t = this, id = args.id;
  if (!id) {
    return callback({msg:'SyncProbe delete - ID not present'});
  }

  // Set the contents of the model for liveSync
  t.getFullPath(id, function(error, response) {
    if (error) {
      return callback({msg:'Error removing file', err:error});
    }
    var fullPath = response.path;
    if (t.has('modelId')) {
      t.set('model', null);
    }

    // Remove the file
    FS.unlink(fullPath, function(error, data) {
      if (error) {
        return callback({msg:'Error removing file'});
      }
      return callback(null, {});
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.getFullPath"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>getFullPath (modelId, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.getFullPath)
- description and source-code
```javascript
getFullPath = function (modelId, callback) {
  var t = this,
      dirPath = t.dirPath;

  // Don't allow relative paths
  var fullPath = Path.join(t.dirPath, modelId);
  if (fullPath.indexOf(dirPath) !== 0) {
    return callback({msg: 'Model ID ' + modelId + ' cannot represent a relative path'});
  }

  // See if the path represents a directory
  FS.stat(fullPath, function(error, stats){

    // If this is an existing directory, return a path to dir/index.json
    if (!error && stats.isDirectory()) {
      return t.getFullPath(modelId + '/index', callback);
    }

    // Normal case - return the path & stat to the json file
    fullPath += '.json';
    FS.stat(fullPath, function(error, stats){

      // Not an error if error == ENOENT
      if (error && error.code === 'ENOENT') {
        error = null; stats = null;
      }

      // Process other FS errors
      if (error) {
        return callback({err: error, msg: "Error while observing file: " + fullPath});
      }

      // Forward the callback
      return callback(null, {path: fullPath, stats: stats});
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (attributes, options){
  var t = this;
  Probe.prototype.initialize.apply(t, arguments);

  // Disable the probe if the root path hasn't been set
  if (!ROOT_PATH) {
    throw new Error('FileSync has not been enabled on this server.');
  }

  // Class name must exist
  if (!t.has('className')) {
    throw new Error('FileSync - Class name not specified');
  }

  // Don't allow a path above the root path
  t.dirPath = Path.join(ROOT_PATH, t.get('className'));
  if (t.dirPath.indexOf(ROOT_PATH) !== 0) {
    throw new Error('Invalid file path');
  }

  // We're done if this isn't a liveSync probe
  if (!t.has('modelId')) {
    return;
  }

  // Assume callback responsibility
  options.asyncInit = true;
  var callback = options.callback;

  // Get the full path to the file
  t.getFullPath(t.get('modelId'), function(error, response){
    if (error) {
      return callback({msg: 'Failed to get the path', err:error});
    }

    // Get the file and stats
    var fullPath = response.path;
    var stats = response.stats;

    // Build the function to watch the file
    var onFileWatch = function(error, content) {

      var isInitializing = (callback !== null),
          initCallback = callback;
      callback = null;

      if (error && error.code === 'ENOENT') {
        // File doesn't exist. Set the model to null.
        t.set({model: {}}, {silent: isInitializing});
        // Convert the code from the sync probe spec
        error.code = 'NOTFOUND';
      }
      if (error) {
        if (isInitializing) {
          t.release();
          var err = {code: error.code, msg: 'LiveSync requires the file to exist and be readable'};
          initCallback(err);
        }
        return;
      }

      // Parse the JSON content into a JS object.
      try {
        content = JSON.parse(content);
        logger.info('fileParse', {id: t.get('modelId'), content: content});
      } catch (e) {

        // Fail the probe on first load error
        if (isInitializing) {
          t.release();
          initCallback({code: 'BAD_FORMAT', msg: 'Non-JSON formatted file'});
        }

        // Nothing productive to do if the file can't be parsed. Just log it.
        logger.error('fileParse', {error: e, id: t.get('modelId'), content: content});
        return;
      }

      // Set the content into the model if it's different
      // Have to compare raw objects because toJSON returns deep references to models
      var priorModel = t.get('model');
      if (!priorModel || !_.isEqual(content, JSON.parse(JSON.stringify(priorModel)))) {
        t.set({model: content}, {silent: isInitializing});
      }

      // Call the initialization callback on first load
      if (isInitializing) {
        initCallback();
      }
    };

    // Load and watch the file
    var watcherOpts = {
      preload: true,
      persistent: true
    };
    t.fileWatcher = FileProbe.watchLoad(fullPath, watcherOpts, onFileWatch);

  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.read_control"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>read_control (args, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.read_control)
- description and source-code
```javascript
read_control = function (args, callback) {
  // Make sure the ID exists
  var t = this, id = args.id;
  if (!id) {
    return callback({msg:'SyncProbe read - ID not present'});
  }

  // Read the file
  t.getFullPath(id, function(error, response){
    if (error) {
      return callback(error);
    }
    if (!response.stats) {
      return callback({code: 'NOTFOUND', msg:'Document with this ID not found'});
    }

    var fullPath = response.path;
    FS.readFile(fullPath, 'utf8', function(error, data) {
      if (error) {
        return callback({code: 'UNKNOWN', msg:'Error reading file', error: error.code});
      }

      // Parse the file
      var model;
      try {
        model = JSON.parse(data);
      } catch (e) {
        return callback({code: 'PARSE', msg: 'Error parsing file'});
      }
      callback(null, model);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>release ()](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.release)
- description and source-code
```javascript
release = function () {
  var t = this;
  if (t.fileWatcher) {
    t.fileWatcher.close();
    t.fileWatcher = null;
  }
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```

#### <a name="apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.update_control"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.FileSyncProbe.prototype.</span>update_control (args, callback)](#apidoc.element.monitor.SyncProbe.FileSyncProbe.prototype.update_control)
- description and source-code
```javascript
update_control = function (args, callback) {

  // Make sure the ID exists
  var t = this, model = args.model;
  if (!model || !model.id) {
    return callback({msg:'SyncProbe create - Data model with ID not present'});
  }

  // Make sure the directory exists
  t.getFullPath(model.id, function(error, response) {
    if (error) {
      return callback(error);
    }

    var fullPath = response.path,
        parentDir = Path.dirname(fullPath);
    FileProbe.mkdir_r(parentDir, function(error) {
      if (error) {
        return callback(error);
      }

      // Set the contents of the model for liveSync
      if (t.has('modelId')) {
        t.set('model', model);
      }

      // Write the file
      FS.writeFile(fullPath, JSON.stringify(model, null, 2), 'utf8', function(error){
        callback(error, {});
      });
    });
  });

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.SyncProbe.prototype"></a>[module monitor.SyncProbe.prototype](#apidoc.module.monitor.SyncProbe.prototype)

#### <a name="apidoc.element.monitor.SyncProbe.prototype.constructor"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>constructor ()](#apidoc.element.monitor.SyncProbe.prototype.constructor)
- description and source-code
```javascript
constructor = function (){ parent.apply(this, arguments); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.prototype.create_control"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>create_control (args, callback)](#apidoc.element.monitor.SyncProbe.prototype.create_control)
- description and source-code
```javascript
create_control = function (args, callback) {
  callback({msg: 'not implemented'});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.prototype.delete_control"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>delete_control (args, callback)](#apidoc.element.monitor.SyncProbe.prototype.delete_control)
- description and source-code
```javascript
delete_control = function (args, callback) {
  callback({msg: 'not implemented'});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.prototype.initialize"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>initialize (attributes, options)](#apidoc.element.monitor.SyncProbe.prototype.initialize)
- description and source-code
```javascript
initialize = function (attributes, options){
  var t = this;
  Probe.prototype.initialize.apply(t, arguments);

  // Determine the probe name based on the class, and coerce this
  // object into one of those by copying all prototype methods.
  var className = t.get('className'),
      config = SyncProbe.Config,
      probeClassName = config.classMap[className] || config.defaultProbe,
      probeClass = SyncProbe[probeClassName];
  _.each(_.functions(probeClass.prototype), function(methodName) {
    t[methodName] = probeClass.prototype[methodName];
  });
  t.probeClass = probeClass.prototype.probeClass;

  // Forward class initialization to the coerced initialize method
  return t.initialize.apply(t, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.prototype.read_control"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>read_control (args, callback)](#apidoc.element.monitor.SyncProbe.prototype.read_control)
- description and source-code
```javascript
read_control = function (args, callback) {
  callback({msg: 'not implemented'});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.SyncProbe.prototype.release"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>release ()](#apidoc.element.monitor.SyncProbe.prototype.release)
- description and source-code
```javascript
release = function () {
  var t = this;
  Probe.prototype.release.apply(t, arguments);
}
```
- example usage
```shell
...
if (error) {
  if (probeImpl) {
    delete t.runningProbesByKey[probeKey];
    delete t.runningProbesById[probeImpl.id];
    try {
      // This may fail depending on how many resources were created
      // by the probe before failure.  Ignore errors.
      probeImpl.release();
    } catch (e){}
  }
  return callback(error);
}

// Probes are released based on reference count
probeImpl.refCount++;
...
```

#### <a name="apidoc.element.monitor.SyncProbe.prototype.update_control"></a>[function <span class="apidocSignatureSpan">monitor.SyncProbe.prototype.</span>update_control (args, callback)](#apidoc.element.monitor.SyncProbe.prototype.update_control)
- description and source-code
```javascript
update_control = function (args, callback) {
  callback({msg: 'not implemented'});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor._"></a>[module monitor._](#apidoc.module.monitor._)

#### <a name="apidoc.element.monitor._._"></a>[function <span class="apidocSignatureSpan">monitor.</span>_ (obj)](#apidoc.element.monitor._._)
- description and source-code
```javascript
_ = function (obj) {
  if (obj instanceof _) return obj;
  if (!(this instanceof _)) return new _(obj);
  this._wrapped = obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.after"></a>[function <span class="apidocSignatureSpan">monitor._.</span>after (times, func)](#apidoc.element.monitor._.after)
- description and source-code
```javascript
after = function (times, func) {
  if (times <= 0) return func();
  return function() {
    if (--times < 1) {
      return func.apply(this, arguments);
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.all"></a>[function <span class="apidocSignatureSpan">monitor._.</span>all (obj, iterator, context)](#apidoc.element.monitor._.all)
- description and source-code
```javascript
all = function (obj, iterator, context) {
  iterator || (iterator = _.identity);
  var result = true;
  if (obj == null) return result;
  if (nativeEvery && obj.every === nativeEvery) return obj.every(iterator, context);
  each(obj, function(value, index, list) {
    if (!(result = result && iterator.call(context, value, index, list))) return breaker;
  });
  return !!result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.any"></a>[function <span class="apidocSignatureSpan">monitor._.</span>any (obj, iterator, context)](#apidoc.element.monitor._.any)
- description and source-code
```javascript
any = function (obj, iterator, context) {
  iterator || (iterator = _.identity);
  var result = false;
  if (obj == null) return result;
  if (nativeSome && obj.some === nativeSome) return obj.some(iterator, context);
  each(obj, function(value, index, list) {
    if (result || (result = iterator.call(context, value, index, list))) return breaker;
  });
  return !!result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.bind"></a>[function <span class="apidocSignatureSpan">monitor._.</span>bind (func, context)](#apidoc.element.monitor._.bind)
- description and source-code
```javascript
bind = function (func, context) {
  if (func.bind === nativeBind && nativeBind) return nativeBind.apply(func, slice.call(arguments, 1));
  var args = slice.call(arguments, 2);
  return function() {
    return func.apply(context, args.concat(slice.call(arguments)));
  };
}
```
- example usage
```shell
...
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
});

// Inbound probe events
t.addEvent('probe:connect', t.probeConnect.bind(t));
t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
t.addEvent('probe:control', t.probeControl.bind(t));

// Connection events
t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
t.addEvent('connection:pong', function(){t.trigger('pong');});
...
```

#### <a name="apidoc.element.monitor._.bindAll"></a>[function <span class="apidocSignatureSpan">monitor._.</span>bindAll (obj)](#apidoc.element.monitor._.bindAll)
- description and source-code
```javascript
bindAll = function (obj) {
  var funcs = slice.call(arguments, 1);
  if (funcs.length === 0) funcs = _.functions(obj);
  each(funcs, function(f) { obj[f] = _.bind(obj[f], obj); });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.chain"></a>[function <span class="apidocSignatureSpan">monitor._.</span>chain (obj)](#apidoc.element.monitor._.chain)
- description and source-code
```javascript
chain = function (obj) {
  return _(obj).chain();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.clone"></a>[function <span class="apidocSignatureSpan">monitor._.</span>clone (obj)](#apidoc.element.monitor._.clone)
- description and source-code
```javascript
clone = function (obj) {
  if (!_.isObject(obj)) return obj;
  return _.isArray(obj) ? obj.slice() : _.extend({}, obj);
}
```
- example usage
```shell
...
        var onConnect = function(error, probe) {
if (error) {return callback(error);}
probeJSON = probe.toJSON();
probeJSON.probeId = probeJSON.id; delete probeJSON.id;
monitor.probe = probe;

// Keep the last known probe state for effective updating
monitor._probeValues = _.clone(probeJSON);

// Perform the initial set silently.  This assures the initial
// probe contents are available on the connect event,
// but doesn't fire a change event before connect.
monitor.set(probeJSON, {silent:true});

// Watch the probe for changes.
...
```

#### <a name="apidoc.element.monitor._.collect"></a>[function <span class="apidocSignatureSpan">monitor._.</span>collect (obj, iterator, context)](#apidoc.element.monitor._.collect)
- description and source-code
```javascript
collect = function (obj, iterator, context) {
  var results = [];
  if (obj == null) return results;
  if (nativeMap && obj.map === nativeMap) return obj.map(iterator, context);
  each(obj, function(value, index, list) {
    results[results.length] = iterator.call(context, value, index, list);
  });
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.compact"></a>[function <span class="apidocSignatureSpan">monitor._.</span>compact (array)](#apidoc.element.monitor._.compact)
- description and source-code
```javascript
compact = function (array) {
  return _.filter(array, _.identity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.compose"></a>[function <span class="apidocSignatureSpan">monitor._.</span>compose ()](#apidoc.element.monitor._.compose)
- description and source-code
```javascript
compose = function () {
  var funcs = arguments;
  return function() {
    var args = arguments;
    for (var i = funcs.length - 1; i >= 0; i--) {
      args = [funcs[i].apply(this, args)];
    }
    return args[0];
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.contains"></a>[function <span class="apidocSignatureSpan">monitor._.</span>contains (obj, target)](#apidoc.element.monitor._.contains)
- description and source-code
```javascript
contains = function (obj, target) {
  if (obj == null) return false;
  if (nativeIndexOf && obj.indexOf === nativeIndexOf) return obj.indexOf(target) != -1;
  return any(obj, function(value) {
    return value === target;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.countBy"></a>[function <span class="apidocSignatureSpan">monitor._.</span>countBy (obj, value, context)](#apidoc.element.monitor._.countBy)
- description and source-code
```javascript
countBy = function (obj, value, context) {
  return group(obj, value, context, function(result, key) {
    if (!_.has(result, key)) result[key] = 0;
    result[key]++;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.debounce"></a>[function <span class="apidocSignatureSpan">monitor._.</span>debounce (func, wait, immediate)](#apidoc.element.monitor._.debounce)
- description and source-code
```javascript
debounce = function (func, wait, immediate) {
  var timeout, result;
  return function() {
    var context = this, args = arguments;
    var later = function() {
      timeout = null;
      if (!immediate) result = func.apply(context, args);
    };
    var callNow = immediate && !timeout;
    clearTimeout(timeout);
    timeout = setTimeout(later, wait);
    if (callNow) result = func.apply(context, args);
    return result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.defaults"></a>[function <span class="apidocSignatureSpan">monitor._.</span>defaults (obj)](#apidoc.element.monitor._.defaults)
- description and source-code
```javascript
defaults = function (obj) {
  each(slice.call(arguments, 1), function(source) {
    if (source) {
      for (var prop in source) {
        if (obj[prop] == null) obj[prop] = source[prop];
      }
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.defer"></a>[function <span class="apidocSignatureSpan">monitor._.</span>defer (func)](#apidoc.element.monitor._.defer)
- description and source-code
```javascript
defer = function (func) {
  return _.delay.apply(_, [func, 1].concat(slice.call(arguments, 1)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.delay"></a>[function <span class="apidocSignatureSpan">monitor._.</span>delay (func, wait)](#apidoc.element.monitor._.delay)
- description and source-code
```javascript
delay = function (func, wait) {
  var args = slice.call(arguments, 2);
  return setTimeout(function(){ return func.apply(null, args); }, wait);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.detect"></a>[function <span class="apidocSignatureSpan">monitor._.</span>detect (obj, iterator, context)](#apidoc.element.monitor._.detect)
- description and source-code
```javascript
detect = function (obj, iterator, context) {
  var result;
  any(obj, function(value, index, list) {
    if (iterator.call(context, value, index, list)) {
      result = value;
      return true;
    }
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.difference"></a>[function <span class="apidocSignatureSpan">monitor._.</span>difference (array)](#apidoc.element.monitor._.difference)
- description and source-code
```javascript
difference = function (array) {
  var rest = concat.apply(ArrayProto, slice.call(arguments, 1));
  return _.filter(array, function(value){ return !_.contains(rest, value); });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.drop"></a>[function <span class="apidocSignatureSpan">monitor._.</span>drop (array, n, guard)](#apidoc.element.monitor._.drop)
- description and source-code
```javascript
drop = function (array, n, guard) {
  return slice.call(array, (n == null) || guard ? 1 : n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.each"></a>[function <span class="apidocSignatureSpan">monitor._.</span>each (obj, iterator, context)](#apidoc.element.monitor._.each)
- description and source-code
```javascript
each = function (obj, iterator, context) {
  if (obj == null) return;
  if (nativeForEach && obj.forEach === nativeForEach) {
    obj.forEach(iterator, context);
  } else if (obj.length === +obj.length) {
    for (var i = 0, l = obj.length; i < l; i++) {
      if (iterator.call(context, obj[i], i, obj) === breaker) return;
    }
  } else {
    for (var key in obj) {
      if (_.has(obj, key)) {
        if (iterator.call(context, obj[key], key, obj) === breaker) return;
      }
    }
  }
}
```
- example usage
```shell
...
  t.addHostCallbacks[hostName].forEach(function(cb) {
    cb(error);
  });
  delete t.addHostCallbacks[hostName];
};

// Build the list of ports already connected
t.connections.each(function(connection){
  var host = connection.get('hostName').toLowerCase();
  var port = connection.get('hostPort');
  if (host === hostName && port >= portStart && port <= portEnd) {
    connectedPorts.push(port);
  }
});
...
```

#### <a name="apidoc.element.monitor._.escape"></a>[function <span class="apidocSignatureSpan">monitor._.</span>escape (string)](#apidoc.element.monitor._.escape)
- description and source-code
```javascript
escape = function (string) {
  if (string == null) return '';
  return ('' + string).replace(entityRegexes[method], function(match) {
    return entityMap[method][match];
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.every"></a>[function <span class="apidocSignatureSpan">monitor._.</span>every (obj, iterator, context)](#apidoc.element.monitor._.every)
- description and source-code
```javascript
every = function (obj, iterator, context) {
  iterator || (iterator = _.identity);
  var result = true;
  if (obj == null) return result;
  if (nativeEvery && obj.every === nativeEvery) return obj.every(iterator, context);
  each(obj, function(value, index, list) {
    if (!(result = result && iterator.call(context, value, index, list))) return breaker;
  });
  return !!result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.extend"></a>[function <span class="apidocSignatureSpan">monitor._.</span>extend (obj)](#apidoc.element.monitor._.extend)
- description and source-code
```javascript
extend = function (obj) {
  each(slice.call(arguments, 1), function(source) {
    if (source) {
      for (var prop in source) {
        obj[prop] = source[prop];
      }
    }
  });
  return obj;
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```

#### <a name="apidoc.element.monitor._.filter"></a>[function <span class="apidocSignatureSpan">monitor._.</span>filter (obj, iterator, context)](#apidoc.element.monitor._.filter)
- description and source-code
```javascript
filter = function (obj, iterator, context) {
  var results = [];
  if (obj == null) return results;
  if (nativeFilter && obj.filter === nativeFilter) return obj.filter(iterator, context);
  each(obj, function(value, index, list) {
    if (iterator.call(context, value, index, list)) results[results.length] = value;
  });
  return results;
}
```
- example usage
```shell
...
    * @protected
    * @param hostName {String} - Host name to search for (null = any host)
    * @param appName {String} - App name to search for (null = any app)
    * @return connections {Array of Connection} - An array of Connection objects matching the criteria
    */
    findConnections: function(hostName, appName) {
      var t = this;
      return t.connections.filter(function(conn) {

// Host or app matches if not specified or if specified and equal
var matchesHost = !hostName || conn.isThisHost(hostName);
var matchesApp = !appName || appName === conn.get('remoteAppName');
var remoteFirewall = conn.get('remoteFirewall');

// This is a match if host + app matches, and it's not firewalled
...
```

#### <a name="apidoc.element.monitor._.find"></a>[function <span class="apidocSignatureSpan">monitor._.</span>find (obj, iterator, context)](#apidoc.element.monitor._.find)
- description and source-code
```javascript
find = function (obj, iterator, context) {
  var result;
  any(obj, function(value, index, list) {
    if (iterator.call(context, value, index, list)) {
      result = value;
      return true;
    }
  });
  return result;
}
```
- example usage
```shell
...
if (t.runningProbesByKey[probeName] || Probe.classes[probeClass] != null) {
  return callback(null, null);
}

// Give named auto-start probes time to start up
var autoStarts = Monitor.Config.Monitor.autoStart;
if (probeName && !probeClass && autoStarts.length) {
  var autoStart = Monitor._.find(autoStarts, function(probeDef) {
    return probeDef.probeName === probeName;
  });
  if (autoStart) {
    setTimeout(function() {
      t.determineConnection(monitorJSON, makeNewConnections, callback);
    },10);
    return;
...
```

#### <a name="apidoc.element.monitor._.findWhere"></a>[function <span class="apidocSignatureSpan">monitor._.</span>findWhere (obj, attrs)](#apidoc.element.monitor._.findWhere)
- description and source-code
```javascript
findWhere = function (obj, attrs) {
  return _.where(obj, attrs, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.first"></a>[function <span class="apidocSignatureSpan">monitor._.</span>first (array, n, guard)](#apidoc.element.monitor._.first)
- description and source-code
```javascript
first = function (array, n, guard) {
  if (array == null) return void 0;
  return (n != null) && !guard ? slice.call(array, 0, n) : array[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.flatten"></a>[function <span class="apidocSignatureSpan">monitor._.</span>flatten (array, shallow)](#apidoc.element.monitor._.flatten)
- description and source-code
```javascript
flatten = function (array, shallow) {
  return flatten(array, shallow, []);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.foldl"></a>[function <span class="apidocSignatureSpan">monitor._.</span>foldl (obj, iterator, memo, context)](#apidoc.element.monitor._.foldl)
- description and source-code
```javascript
foldl = function (obj, iterator, memo, context) {
  var initial = arguments.length > 2;
  if (obj == null) obj = [];
  if (nativeReduce && obj.reduce === nativeReduce) {
    if (context) iterator = _.bind(iterator, context);
    return initial ? obj.reduce(iterator, memo) : obj.reduce(iterator);
  }
  each(obj, function(value, index, list) {
    if (!initial) {
      memo = value;
      initial = true;
    } else {
      memo = iterator.call(context, memo, value, index, list);
    }
  });
  if (!initial) throw new TypeError(reduceError);
  return memo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.foldr"></a>[function <span class="apidocSignatureSpan">monitor._.</span>foldr (obj, iterator, memo, context)](#apidoc.element.monitor._.foldr)
- description and source-code
```javascript
foldr = function (obj, iterator, memo, context) {
  var initial = arguments.length > 2;
  if (obj == null) obj = [];
  if (nativeReduceRight && obj.reduceRight === nativeReduceRight) {
    if (context) iterator = _.bind(iterator, context);
    return initial ? obj.reduceRight(iterator, memo) : obj.reduceRight(iterator);
  }
  var length = obj.length;
  if (length !== +length) {
    var keys = _.keys(obj);
    length = keys.length;
  }
  each(obj, function(value, index, list) {
    index = keys ? keys[--length] : --length;
    if (!initial) {
      memo = obj[index];
      initial = true;
    } else {
      memo = iterator.call(context, memo, obj[index], index, list);
    }
  });
  if (!initial) throw new TypeError(reduceError);
  return memo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.forEach"></a>[function <span class="apidocSignatureSpan">monitor._.</span>forEach (obj, iterator, context)](#apidoc.element.monitor._.forEach)
- description and source-code
```javascript
forEach = function (obj, iterator, context) {
  if (obj == null) return;
  if (nativeForEach && obj.forEach === nativeForEach) {
    obj.forEach(iterator, context);
  } else if (obj.length === +obj.length) {
    for (var i = 0, l = obj.length; i < l; i++) {
      if (iterator.call(context, obj[i], i, obj) === breaker) return;
    }
  } else {
    for (var key in obj) {
      if (_.has(obj, key)) {
        if (iterator.call(context, obj[key], key, obj) === breaker) return;
      }
    }
  }
}
```
- example usage
```shell
...

  // Allow probes to be externally identified by name
  if (probeJSON.probeName) {
    return probeJSON.probeName;
  }

  if (initParams) {
    _.keys(initParams).sort().forEach(function(key){
      probeKey += ':' + key + '=' + initParams[key];
    });
  }
  return probeKey;
},

/**
...
```

#### <a name="apidoc.element.monitor._.functions"></a>[function <span class="apidocSignatureSpan">monitor._.</span>functions (obj)](#apidoc.element.monitor._.functions)
- description and source-code
```javascript
functions = function (obj) {
  var names = [];
  for (var key in obj) {
    if (_.isFunction(obj[key])) names.push(key);
  }
  return names.sort();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.groupBy"></a>[function <span class="apidocSignatureSpan">monitor._.</span>groupBy (obj, value, context)](#apidoc.element.monitor._.groupBy)
- description and source-code
```javascript
groupBy = function (obj, value, context) {
  return group(obj, value, context, function(result, key, value) {
    (_.has(result, key) ? result[key] : (result[key] = [])).push(value);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.has"></a>[function <span class="apidocSignatureSpan">monitor._.</span>has (obj, key)](#apidoc.element.monitor._.has)
- description and source-code
```javascript
has = function (obj, key) {
  return hasOwnProperty.call(obj, key);
}
```
- example usage
```shell
...

// Cannot liveSync with a collection (too many issues)
if (options.liveSync && model instanceof Backbone.Collection) {
  return options.error(null, 'Cannot liveSync with a collection');
}

// Generate an ID if necessary
if (!model.has('id')) {
  if (method === METHOD_CREATE) {
    model.set({id: Monitor.generateUniqueId()}, {silent: true});
    logger.info('_sync.generateUniqueId', t.className, model.toJSON(), options);
  } else {
    return options.error(null, 'ID element must be set.');
  }
}
...
```

#### <a name="apidoc.element.monitor._.head"></a>[function <span class="apidocSignatureSpan">monitor._.</span>head (array, n, guard)](#apidoc.element.monitor._.head)
- description and source-code
```javascript
head = function (array, n, guard) {
  if (array == null) return void 0;
  return (n != null) && !guard ? slice.call(array, 0, n) : array[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.identity"></a>[function <span class="apidocSignatureSpan">monitor._.</span>identity (value)](#apidoc.element.monitor._.identity)
- description and source-code
```javascript
identity = function (value) {
  return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.include"></a>[function <span class="apidocSignatureSpan">monitor._.</span>include (obj, target)](#apidoc.element.monitor._.include)
- description and source-code
```javascript
include = function (obj, target) {
  if (obj == null) return false;
  if (nativeIndexOf && obj.indexOf === nativeIndexOf) return obj.indexOf(target) != -1;
  return any(obj, function(value) {
    return value === target;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.indexOf"></a>[function <span class="apidocSignatureSpan">monitor._.</span>indexOf (array, item, isSorted)](#apidoc.element.monitor._.indexOf)
- description and source-code
```javascript
indexOf = function (array, item, isSorted) {
  if (array == null) return -1;
  var i = 0, l = array.length;
  if (isSorted) {
    if (typeof isSorted == 'number') {
      i = (isSorted < 0 ? Math.max(0, l + isSorted) : isSorted);
    } else {
      i = _.sortedIndex(array, item);
      return array[i] === item ? i : -1;
    }
  }
  if (nativeIndexOf && array.indexOf === nativeIndexOf) return array.indexOf(item, isSorted);
  for (; i < l; i++) if (array[i] === item) return i;
  return -1;
}
```
- example usage
```shell
...
    set_control: function(attrs, callback) {
var t = this,
    writableAttributes = t.get('writableAttributes') || [];

// Validate the attributes are writable
if (writableAttributes !== '*') {
  for (var attrName in attrs) {
    if (writableAttributes.indexOf(attrName) < 0) {
      return callback({code:'NOT_WRITABLE', msg: 'Attribute not writable: ' + attrName});
    }
  }
}

// Set the data
var error = null;
...
```

#### <a name="apidoc.element.monitor._.initial"></a>[function <span class="apidocSignatureSpan">monitor._.</span>initial (array, n, guard)](#apidoc.element.monitor._.initial)
- description and source-code
```javascript
initial = function (array, n, guard) {
  return slice.call(array, 0, array.length - ((n == null) || guard ? 1 : n));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.inject"></a>[function <span class="apidocSignatureSpan">monitor._.</span>inject (obj, iterator, memo, context)](#apidoc.element.monitor._.inject)
- description and source-code
```javascript
inject = function (obj, iterator, memo, context) {
  var initial = arguments.length > 2;
  if (obj == null) obj = [];
  if (nativeReduce && obj.reduce === nativeReduce) {
    if (context) iterator = _.bind(iterator, context);
    return initial ? obj.reduce(iterator, memo) : obj.reduce(iterator);
  }
  each(obj, function(value, index, list) {
    if (!initial) {
      memo = value;
      initial = true;
    } else {
      memo = iterator.call(context, memo, value, index, list);
    }
  });
  if (!initial) throw new TypeError(reduceError);
  return memo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.intersection"></a>[function <span class="apidocSignatureSpan">monitor._.</span>intersection (array)](#apidoc.element.monitor._.intersection)
- description and source-code
```javascript
intersection = function (array) {
  var rest = slice.call(arguments, 1);
  return _.filter(_.uniq(array), function(item) {
    return _.every(rest, function(other) {
      return _.indexOf(other, item) >= 0;
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.invert"></a>[function <span class="apidocSignatureSpan">monitor._.</span>invert (obj)](#apidoc.element.monitor._.invert)
- description and source-code
```javascript
invert = function (obj) {
  var result = {};
  for (var key in obj) if (_.has(obj, key)) result[obj[key]] = key;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.invoke"></a>[function <span class="apidocSignatureSpan">monitor._.</span>invoke (obj, method)](#apidoc.element.monitor._.invoke)
- description and source-code
```javascript
invoke = function (obj, method) {
  var args = slice.call(arguments, 2);
  var isFunc = _.isFunction(method);
  return _.map(obj, function(value) {
    return (isFunc ? method : value[method]).apply(value, args);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isArguments"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isArguments (obj)](#apidoc.element.monitor._.isArguments)
- description and source-code
```javascript
isArguments = function (obj) {
  return toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isArray"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isArray ()](#apidoc.element.monitor._.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isBoolean"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isBoolean (obj)](#apidoc.element.monitor._.isBoolean)
- description and source-code
```javascript
isBoolean = function (obj) {
  return obj === true || obj === false || toString.call(obj) == '[object Boolean]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isDate"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isDate (obj)](#apidoc.element.monitor._.isDate)
- description and source-code
```javascript
isDate = function (obj) {
  return toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isElement"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isElement (obj)](#apidoc.element.monitor._.isElement)
- description and source-code
```javascript
isElement = function (obj) {
  return !!(obj && obj.nodeType === 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isEmpty"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isEmpty (obj)](#apidoc.element.monitor._.isEmpty)
- description and source-code
```javascript
isEmpty = function (obj) {
  if (obj == null) return true;
  if (_.isArray(obj) || _.isString(obj)) return obj.length === 0;
  for (var key in obj) if (_.has(obj, key)) return false;
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isEqual"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isEqual (a, b)](#apidoc.element.monitor._.isEqual)
- description and source-code
```javascript
isEqual = function (a, b) {
  return eq(a, b, [], []);
}
```
- example usage
```shell
...
      };

      // Client-side listener - for persisting changes to the server
      var modelListener = function(changedModel, options) {
options = options || {};

// Don't persist unless the model is different
if (_.isEqual(JSON.parse(JSON.stringify(model)), JSON.parse(JSON.stringify(model.syncMonitor.get('model'))))) {
  logger.info('modelListener.noChanges', t.className, model.toJSON());
  return;
}

// Disconnect listeners if the ID changes
if (model.get('id') !== modelId) {
  logger.info('modelListener.alteredId', t.className, model.toJSON());
...
```

#### <a name="apidoc.element.monitor._.isFinite"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isFinite (obj)](#apidoc.element.monitor._.isFinite)
- description and source-code
```javascript
isFinite = function (obj) {
  return isFinite(obj) && !isNaN(parseFloat(obj));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isFunction"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isFunction (obj)](#apidoc.element.monitor._.isFunction)
- description and source-code
```javascript
isFunction = function (obj) {
  return typeof obj === 'function';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isNaN"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isNaN (obj)](#apidoc.element.monitor._.isNaN)
- description and source-code
```javascript
isNaN = function (obj) {
  return _.isNumber(obj) && obj != +obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isNull"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isNull (obj)](#apidoc.element.monitor._.isNull)
- description and source-code
```javascript
isNull = function (obj) {
  return obj === null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isNumber"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isNumber (obj)](#apidoc.element.monitor._.isNumber)
- description and source-code
```javascript
isNumber = function (obj) {
  return toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
...
* for maintaining the prior and new value for the stat.
*
* @method increment
* @param name {String} Dot.separated name of the counter to increment
* @param [value=1] {Number} Amount to increment the counter by.
*/
proto.increment = function(name, value){
  value = _.isNumber(value) ? value : 1;
  Stat._emit(this.module, name, value, 'c');
};

/**
* Decrement a counter by a specified value
*
* Assuming someone is listening to this stat, this is an instruction for that
...
```

#### <a name="apidoc.element.monitor._.isObject"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isObject (obj)](#apidoc.element.monitor._.isObject)
- description and source-code
```javascript
isObject = function (obj) {
  return obj === Object(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isRegExp"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isRegExp (obj)](#apidoc.element.monitor._.isRegExp)
- description and source-code
```javascript
isRegExp = function (obj) {
  return toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isString"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isString (obj)](#apidoc.element.monitor._.isString)
- description and source-code
```javascript
isString = function (obj) {
  return toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.isUndefined"></a>[function <span class="apidocSignatureSpan">monitor._.</span>isUndefined (obj)](#apidoc.element.monitor._.isUndefined)
- description and source-code
```javascript
isUndefined = function (obj) {
  return obj === void 0;
}
```
- example usage
```shell
...
    * @return connection {Connection} - The added connection
    */
    addConnection: function(options) {
var t = this,
    startTime = Date.now();

// Default the firewall value
if (_.isUndefined(options.firewall)) {
  options = _.extend({},options, {firewall: t.firewall});
}

// Generate a unique ID for the connection
options.id = Monitor.generateUniqueCollectionId(t.connections);

var connStr = 'Conn_' + options.id;
...
```

#### <a name="apidoc.element.monitor._.keys"></a>[function <span class="apidocSignatureSpan">monitor._.</span>keys ()](#apidoc.element.monitor._.keys)
- description and source-code
```javascript
function keys() { [native code] }
```
- example usage
```shell
...

  // Exchange connection information
  socket.emit('connection:info', {
    hostName:Monitor.getRouter().getHostName(),
    appName:Config.Monitor.appName,
    appInstance: appInstance,
    pid: pid,
    probeClasses: _.keys(Probe.classes),
    gateway:t.get('gateway'),
    firewall:t.get('firewall')
  });
},

/**
* Process an inbound request to connect with a probe
...
```

#### <a name="apidoc.element.monitor._.last"></a>[function <span class="apidocSignatureSpan">monitor._.</span>last (array, n, guard)](#apidoc.element.monitor._.last)
- description and source-code
```javascript
last = function (array, n, guard) {
  if (array == null) return void 0;
  if ((n != null) && !guard) {
    return slice.call(array, Math.max(array.length - n, 0));
  } else {
    return array[array.length - 1];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.lastIndexOf"></a>[function <span class="apidocSignatureSpan">monitor._.</span>lastIndexOf (array, item, from)](#apidoc.element.monitor._.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function (array, item, from) {
  if (array == null) return -1;
  var hasIndex = from != null;
  if (nativeLastIndexOf && array.lastIndexOf === nativeLastIndexOf) {
    return hasIndex ? array.lastIndexOf(item, from) : array.lastIndexOf(item);
  }
  var i = (hasIndex ? from : array.length);
  while (i--) if (array[i] === item) return i;
  return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.map"></a>[function <span class="apidocSignatureSpan">monitor._.</span>map (obj, iterator, context)](#apidoc.element.monitor._.map)
- description and source-code
```javascript
map = function (obj, iterator, context) {
  var results = [];
  if (obj == null) return results;
  if (nativeMap && obj.map === nativeMap) return obj.map(iterator, context);
  each(obj, function(value, index, list) {
    results[results.length] = iterator.call(context, value, index, list);
  });
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.max"></a>[function <span class="apidocSignatureSpan">monitor._.</span>max (obj, iterator, context)](#apidoc.element.monitor._.max)
- description and source-code
```javascript
max = function (obj, iterator, context) {
  if (!iterator && _.isArray(obj) && obj[0] === +obj[0] && obj.length < 65535) {
    return Math.max.apply(Math, obj);
  }
  if (!iterator && _.isEmpty(obj)) return -Infinity;
  var result = {computed : -Infinity, value: -Infinity};
  each(obj, function(value, index, list) {
    var computed = iterator ? iterator.call(context, value, index, list) : value;
    computed >= result.computed && (result = {value : value, computed : computed});
  });
  return result.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.memoize"></a>[function <span class="apidocSignatureSpan">monitor._.</span>memoize (func, hasher)](#apidoc.element.monitor._.memoize)
- description and source-code
```javascript
memoize = function (func, hasher) {
  var memo = {};
  hasher || (hasher = _.identity);
  return function() {
    var key = hasher.apply(this, arguments);
    return _.has(memo, key) ? memo[key] : (memo[key] = func.apply(this, arguments));
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.methods"></a>[function <span class="apidocSignatureSpan">monitor._.</span>methods (obj)](#apidoc.element.monitor._.methods)
- description and source-code
```javascript
methods = function (obj) {
  var names = [];
  for (var key in obj) {
    if (_.isFunction(obj[key])) names.push(key);
  }
  return names.sort();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.min"></a>[function <span class="apidocSignatureSpan">monitor._.</span>min (obj, iterator, context)](#apidoc.element.monitor._.min)
- description and source-code
```javascript
min = function (obj, iterator, context) {
  if (!iterator && _.isArray(obj) && obj[0] === +obj[0] && obj.length < 65535) {
    return Math.min.apply(Math, obj);
  }
  if (!iterator && _.isEmpty(obj)) return Infinity;
  var result = {computed : Infinity, value: Infinity};
  each(obj, function(value, index, list) {
    var computed = iterator ? iterator.call(context, value, index, list) : value;
    computed < result.computed && (result = {value : value, computed : computed});
  });
  return result.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.mixin"></a>[function <span class="apidocSignatureSpan">monitor._.</span>mixin (obj)](#apidoc.element.monitor._.mixin)
- description and source-code
```javascript
mixin = function (obj) {
  each(_.functions(obj), function(name){
    var func = _[name] = obj[name];
    _.prototype[name] = function() {
      var args = [this._wrapped];
      push.apply(args, arguments);
      return result.call(this, func.apply(_, args));
    };
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.noConflict"></a>[function <span class="apidocSignatureSpan">monitor._.</span>noConflict ()](#apidoc.element.monitor._.noConflict)
- description and source-code
```javascript
noConflict = function () {
  root._ = previousUnderscore;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.object"></a>[function <span class="apidocSignatureSpan">monitor._.</span>object (list, values)](#apidoc.element.monitor._.object)
- description and source-code
```javascript
object = function (list, values) {
  if (list == null) return {};
  var result = {};
  for (var i = 0, l = list.length; i < l; i++) {
    if (values) {
      result[list[i]] = values[i];
    } else {
      result[list[i][0]] = list[i][1];
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.omit"></a>[function <span class="apidocSignatureSpan">monitor._.</span>omit (obj)](#apidoc.element.monitor._.omit)
- description and source-code
```javascript
omit = function (obj) {
  var copy = {};
  var keys = concat.apply(ArrayProto, slice.call(arguments, 1));
  for (var key in obj) {
    if (!_.contains(keys, key)) copy[key] = obj[key];
  }
  return copy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.once"></a>[function <span class="apidocSignatureSpan">monitor._.</span>once (func)](#apidoc.element.monitor._.once)
- description and source-code
```javascript
once = function (func) {
  var ran = false, memo;
  return function() {
    if (ran) return memo;
    ran = true;
    memo = func.apply(this, arguments);
    func = null;
    return memo;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.pairs"></a>[function <span class="apidocSignatureSpan">monitor._.</span>pairs (obj)](#apidoc.element.monitor._.pairs)
- description and source-code
```javascript
pairs = function (obj) {
  var pairs = [];
  for (var key in obj) if (_.has(obj, key)) pairs.push([key, obj[key]]);
  return pairs;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.partial"></a>[function <span class="apidocSignatureSpan">monitor._.</span>partial (func)](#apidoc.element.monitor._.partial)
- description and source-code
```javascript
partial = function (func) {
  var args = slice.call(arguments, 1);
  return function() {
    return func.apply(this, args.concat(slice.call(arguments)));
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.pick"></a>[function <span class="apidocSignatureSpan">monitor._.</span>pick (obj)](#apidoc.element.monitor._.pick)
- description and source-code
```javascript
pick = function (obj) {
  var copy = {};
  var keys = concat.apply(ArrayProto, slice.call(arguments, 1));
  each(keys, function(key) {
    if (key in obj) copy[key] = obj[key];
  });
  return copy;
}
```
- example usage
```shell
...
  *   params for the class.
  * @return {Object} The monitor parameters
  */
  Sync.prototype._getMonitorParams = function(modelId) {

// Build server connection parameters from this instance of Sync
var t = this;
var params = _.pick(t.options, 'hostName', 'appName', 'appInstance');

// Add probe and class parameters
params.probeClass = 'Sync';
params.initParams = {
  className: t.className
};
...
```

#### <a name="apidoc.element.monitor._.pluck"></a>[function <span class="apidocSignatureSpan">monitor._.</span>pluck (obj, key)](#apidoc.element.monitor._.pluck)
- description and source-code
```javascript
pluck = function (obj, key) {
  return _.map(obj, function(value){ return value[key]; });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.random"></a>[function <span class="apidocSignatureSpan">monitor._.</span>random (min, max)](#apidoc.element.monitor._.random)
- description and source-code
```javascript
random = function (min, max) {
  if (max == null) {
    max = min;
    min = 0;
  }
  return min + Math.floor(Math.random() * (max - min + 1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.range"></a>[function <span class="apidocSignatureSpan">monitor._.</span>range (start, stop, step)](#apidoc.element.monitor._.range)
- description and source-code
```javascript
range = function (start, stop, step) {
  if (arguments.length <= 1) {
    stop = start || 0;
    start = 0;
  }
  step = arguments[2] || 1;

  var len = Math.max(Math.ceil((stop - start) / step), 0);
  var idx = 0;
  var range = new Array(len);

  while(idx < len) {
    range[idx++] = start;
    start += step;
  }

  return range;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.reduce"></a>[function <span class="apidocSignatureSpan">monitor._.</span>reduce (obj, iterator, memo, context)](#apidoc.element.monitor._.reduce)
- description and source-code
```javascript
reduce = function (obj, iterator, memo, context) {
  var initial = arguments.length > 2;
  if (obj == null) obj = [];
  if (nativeReduce && obj.reduce === nativeReduce) {
    if (context) iterator = _.bind(iterator, context);
    return initial ? obj.reduce(iterator, memo) : obj.reduce(iterator);
  }
  each(obj, function(value, index, list) {
    if (!initial) {
      memo = value;
      initial = true;
    } else {
      memo = iterator.call(context, memo, value, index, list);
    }
  });
  if (!initial) throw new TypeError(reduceError);
  return memo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.reduceRight"></a>[function <span class="apidocSignatureSpan">monitor._.</span>reduceRight (obj, iterator, memo, context)](#apidoc.element.monitor._.reduceRight)
- description and source-code
```javascript
reduceRight = function (obj, iterator, memo, context) {
  var initial = arguments.length > 2;
  if (obj == null) obj = [];
  if (nativeReduceRight && obj.reduceRight === nativeReduceRight) {
    if (context) iterator = _.bind(iterator, context);
    return initial ? obj.reduceRight(iterator, memo) : obj.reduceRight(iterator);
  }
  var length = obj.length;
  if (length !== +length) {
    var keys = _.keys(obj);
    length = keys.length;
  }
  each(obj, function(value, index, list) {
    index = keys ? keys[--length] : --length;
    if (!initial) {
      memo = obj[index];
      initial = true;
    } else {
      memo = iterator.call(context, memo, obj[index], index, list);
    }
  });
  if (!initial) throw new TypeError(reduceError);
  return memo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.reject"></a>[function <span class="apidocSignatureSpan">monitor._.</span>reject (obj, iterator, context)](#apidoc.element.monitor._.reject)
- description and source-code
```javascript
reject = function (obj, iterator, context) {
  return _.filter(obj, function(value, index, list) {
    return !iterator.call(context, value, index, list);
  }, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.rest"></a>[function <span class="apidocSignatureSpan">monitor._.</span>rest (array, n, guard)](#apidoc.element.monitor._.rest)
- description and source-code
```javascript
rest = function (array, n, guard) {
  return slice.call(array, (n == null) || guard ? 1 : n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.result"></a>[function <span class="apidocSignatureSpan">monitor._.</span>result (object, property)](#apidoc.element.monitor._.result)
- description and source-code
```javascript
result = function (object, property) {
  if (object == null) return null;
  var value = object[property];
  return _.isFunction(value) ? value.call(object) : value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.select"></a>[function <span class="apidocSignatureSpan">monitor._.</span>select (obj, iterator, context)](#apidoc.element.monitor._.select)
- description and source-code
```javascript
select = function (obj, iterator, context) {
  var results = [];
  if (obj == null) return results;
  if (nativeFilter && obj.filter === nativeFilter) return obj.filter(iterator, context);
  each(obj, function(value, index, list) {
    if (iterator.call(context, value, index, list)) results[results.length] = value;
  });
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.shuffle"></a>[function <span class="apidocSignatureSpan">monitor._.</span>shuffle (obj)](#apidoc.element.monitor._.shuffle)
- description and source-code
```javascript
shuffle = function (obj) {
  var rand;
  var index = 0;
  var shuffled = [];
  each(obj, function(value) {
    rand = _.random(index++);
    shuffled[index - 1] = shuffled[rand];
    shuffled[rand] = value;
  });
  return shuffled;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.size"></a>[function <span class="apidocSignatureSpan">monitor._.</span>size (obj)](#apidoc.element.monitor._.size)
- description and source-code
```javascript
size = function (obj) {
  if (obj == null) return 0;
  return (obj.length === +obj.length) ? obj.length : _.keys(obj).length;
}
```
- example usage
```shell
...
var newModel = model.syncMonitor.get('model');
if (_.isEqual(JSON.parse(JSON.stringify(model)), JSON.parse(JSON.stringify(newModel)))) {
  logger.info('monitorListener.noChanges', t.className, newModel);
  return;
}

// Disconnect if the model was deleted or the ID isn't the same
var isDeleted = (_.size(newModel) === 0);
if (isDeleted || newModel.id !== modelId)  {
  logger.info('modelListener.deleted', t.className, newModel);
  disconnectListeners();
}

// Forward changes to the model (including server-side delete)
var newOpts = {isSyncChanging:true};
...
```

#### <a name="apidoc.element.monitor._.some"></a>[function <span class="apidocSignatureSpan">monitor._.</span>some (obj, iterator, context)](#apidoc.element.monitor._.some)
- description and source-code
```javascript
some = function (obj, iterator, context) {
  iterator || (iterator = _.identity);
  var result = false;
  if (obj == null) return result;
  if (nativeSome && obj.some === nativeSome) return obj.some(iterator, context);
  each(obj, function(value, index, list) {
    if (result || (result = iterator.call(context, value, index, list))) return breaker;
  });
  return !!result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.sortBy"></a>[function <span class="apidocSignatureSpan">monitor._.</span>sortBy (obj, value, context)](#apidoc.element.monitor._.sortBy)
- description and source-code
```javascript
sortBy = function (obj, value, context) {
  var iterator = lookupIterator(value);
  return _.pluck(_.map(obj, function(value, index, list) {
    return {
      value : value,
      index : index,
      criteria : iterator.call(context, value, index, list)
    };
  }).sort(function(left, right) {
    var a = left.criteria;
    var b = right.criteria;
    if (a !== b) {
      if (a > b || a === void 0) return 1;
      if (a < b || b === void 0) return -1;
    }
    return left.index < right.index ? -1 : 1;
  }), 'value');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.sortedIndex"></a>[function <span class="apidocSignatureSpan">monitor._.</span>sortedIndex (array, obj, iterator, context)](#apidoc.element.monitor._.sortedIndex)
- description and source-code
```javascript
sortedIndex = function (array, obj, iterator, context) {
  iterator = iterator == null ? _.identity : lookupIterator(iterator);
  var value = iterator.call(context, obj);
  var low = 0, high = array.length;
  while (low < high) {
    var mid = (low + high) >>> 1;
    iterator.call(context, array[mid]) < value ? low = mid + 1 : high = mid;
  }
  return low;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.tail"></a>[function <span class="apidocSignatureSpan">monitor._.</span>tail (array, n, guard)](#apidoc.element.monitor._.tail)
- description and source-code
```javascript
tail = function (array, n, guard) {
  return slice.call(array, (n == null) || guard ? 1 : n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.take"></a>[function <span class="apidocSignatureSpan">monitor._.</span>take (array, n, guard)](#apidoc.element.monitor._.take)
- description and source-code
```javascript
take = function (array, n, guard) {
  if (array == null) return void 0;
  return (n != null) && !guard ? slice.call(array, 0, n) : array[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.tap"></a>[function <span class="apidocSignatureSpan">monitor._.</span>tap (obj, interceptor)](#apidoc.element.monitor._.tap)
- description and source-code
```javascript
tap = function (obj, interceptor) {
  interceptor(obj);
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.template"></a>[function <span class="apidocSignatureSpan">monitor._.</span>template (text, data, settings)](#apidoc.element.monitor._.template)
- description and source-code
```javascript
template = function (text, data, settings) {
  var render;
  settings = _.defaults({}, settings, _.templateSettings);

  // Combine delimiters into one regular expression via alternation.
  var matcher = new RegExp([
    (settings.escape || noMatch).source,
    (settings.interpolate || noMatch).source,
    (settings.evaluate || noMatch).source
  ].join('|') + '|$', 'g');

  // Compile the template source, escaping string literals appropriately.
  var index = 0;
  var source = "__p+='";
  text.replace(matcher, function(match, escape, interpolate, evaluate, offset) {
    source += text.slice(index, offset)
      .replace(escaper, function(match) { return '\\' + escapes[match]; });

    if (escape) {
      source += "'+\n((__t=(" + escape + "))==null?'':_.escape(__t))+\n'";
    }
    if (interpolate) {
      source += "'+\n((__t=(" + interpolate + "))==null?'':__t)+\n'";
    }
    if (evaluate) {
      source += "';\n" + evaluate + "\n__p+='";
    }
    index = offset + match.length;
    return match;
  });
  source += "';\n";

  // If a variable is not specified, place data values in local scope.
  if (!settings.variable) source = 'with(obj||{}){\n' + source + '}\n';

  source = "var __t,__p='',__j=Array.prototype.join," +
    "print=function(){__p+=__j.call(arguments,'');};\n" +
    source + "return __p;\n";

  try {
    render = new Function(settings.variable || 'obj', '_', source);
  } catch (e) {
    e.source = source;
    throw e;
  }

  if (data) return render(data, _);
  var template = function(data) {
    return render.call(this, data, _);
  };

  // Provide the compiled function source as a convenience for precompilation.
  template.source = 'function(' + (settings.variable || 'obj') + '){\n' + source + '}';

  return template;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.throttle"></a>[function <span class="apidocSignatureSpan">monitor._.</span>throttle (func, wait)](#apidoc.element.monitor._.throttle)
- description and source-code
```javascript
throttle = function (func, wait) {
  var context, args, timeout, result;
  var previous = 0;
  var later = function() {
    previous = new Date;
    timeout = null;
    result = func.apply(context, args);
  };
  return function() {
    var now = new Date;
    var remaining = wait - (now - previous);
    context = this;
    args = arguments;
    if (remaining <= 0) {
      clearTimeout(timeout);
      timeout = null;
      previous = now;
      result = func.apply(context, args);
    } else if (!timeout) {
      timeout = setTimeout(later, remaining);
    }
    return result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.times"></a>[function <span class="apidocSignatureSpan">monitor._.</span>times (n, iterator, context)](#apidoc.element.monitor._.times)
- description and source-code
```javascript
times = function (n, iterator, context) {
  var accum = Array(n);
  for (var i = 0; i < n; i++) accum[i] = iterator.call(context, i);
  return accum;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.toArray"></a>[function <span class="apidocSignatureSpan">monitor._.</span>toArray (obj)](#apidoc.element.monitor._.toArray)
- description and source-code
```javascript
toArray = function (obj) {
  if (!obj) return [];
  if (_.isArray(obj)) return slice.call(obj);
  if (obj.length === +obj.length) return _.map(obj, _.identity);
  return _.values(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.unescape"></a>[function <span class="apidocSignatureSpan">monitor._.</span>unescape (string)](#apidoc.element.monitor._.unescape)
- description and source-code
```javascript
unescape = function (string) {
  if (string == null) return '';
  return ('' + string).replace(entityRegexes[method], function(match) {
    return entityMap[method][match];
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.union"></a>[function <span class="apidocSignatureSpan">monitor._.</span>union ()](#apidoc.element.monitor._.union)
- description and source-code
```javascript
union = function () {
  return _.uniq(concat.apply(ArrayProto, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.uniq"></a>[function <span class="apidocSignatureSpan">monitor._.</span>uniq (array, isSorted, iterator, context)](#apidoc.element.monitor._.uniq)
- description and source-code
```javascript
uniq = function (array, isSorted, iterator, context) {
  if (_.isFunction(isSorted)) {
    context = iterator;
    iterator = isSorted;
    isSorted = false;
  }
  var initial = iterator ? _.map(array, iterator, context) : array;
  var results = [];
  var seen = [];
  each(initial, function(value, index) {
    if (isSorted ? (!index || seen[seen.length - 1] !== value) : !_.contains(seen, value)) {
      seen.push(value);
      results.push(array[index]);
    }
  });
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.unique"></a>[function <span class="apidocSignatureSpan">monitor._.</span>unique (array, isSorted, iterator, context)](#apidoc.element.monitor._.unique)
- description and source-code
```javascript
unique = function (array, isSorted, iterator, context) {
  if (_.isFunction(isSorted)) {
    context = iterator;
    iterator = isSorted;
    isSorted = false;
  }
  var initial = iterator ? _.map(array, iterator, context) : array;
  var results = [];
  var seen = [];
  each(initial, function(value, index) {
    if (isSorted ? (!index || seen[seen.length - 1] !== value) : !_.contains(seen, value)) {
      seen.push(value);
      results.push(array[index]);
    }
  });
  return results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.uniqueId"></a>[function <span class="apidocSignatureSpan">monitor._.</span>uniqueId (prefix)](#apidoc.element.monitor._.uniqueId)
- description and source-code
```javascript
uniqueId = function (prefix) {
  var id = ++idCounter + '';
  return prefix ? prefix + id : id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.values"></a>[function <span class="apidocSignatureSpan">monitor._.</span>values (obj)](#apidoc.element.monitor._.values)
- description and source-code
```javascript
values = function (obj) {
  var values = [];
  for (var key in obj) if (_.has(obj, key)) values.push(obj[key]);
  return values;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.where"></a>[function <span class="apidocSignatureSpan">monitor._.</span>where (obj, attrs, first)](#apidoc.element.monitor._.where)
- description and source-code
```javascript
where = function (obj, attrs, first) {
  if (_.isEmpty(attrs)) return first ? null : [];
  return _[first ? 'find' : 'filter'](obj, function(value) {
    for (var key in attrs) {
      if (attrs[key] !== value[key]) return false;
    }
    return true;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.without"></a>[function <span class="apidocSignatureSpan">monitor._.</span>without (array)](#apidoc.element.monitor._.without)
- description and source-code
```javascript
without = function (array) {
  return _.difference(array, slice.call(arguments, 1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.wrap"></a>[function <span class="apidocSignatureSpan">monitor._.</span>wrap (func, wrapper)](#apidoc.element.monitor._.wrap)
- description and source-code
```javascript
wrap = function (func, wrapper) {
  return function() {
    var args = [func];
    push.apply(args, arguments);
    return wrapper.apply(this, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.zip"></a>[function <span class="apidocSignatureSpan">monitor._.</span>zip ()](#apidoc.element.monitor._.zip)
- description and source-code
```javascript
zip = function () {
  var args = slice.call(arguments);
  var length = _.max(_.pluck(args, 'length'));
  var results = new Array(length);
  for (var i = 0; i < length; i++) {
    results[i] = _.pluck(args, "" + i);
  }
  return results;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor._.prototype"></a>[module monitor._.prototype](#apidoc.module.monitor._.prototype)

#### <a name="apidoc.element.monitor._.prototype._"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>_ ()](#apidoc.element.monitor._.prototype._)
- description and source-code
```javascript
_ = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.after"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>after ()](#apidoc.element.monitor._.prototype.after)
- description and source-code
```javascript
after = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.all"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>all ()](#apidoc.element.monitor._.prototype.all)
- description and source-code
```javascript
all = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.any"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>any ()](#apidoc.element.monitor._.prototype.any)
- description and source-code
```javascript
any = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.bind"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>bind ()](#apidoc.element.monitor._.prototype.bind)
- description and source-code
```javascript
bind = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
});

// Inbound probe events
t.addEvent('probe:connect', t.probeConnect.bind(t));
t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
t.addEvent('probe:control', t.probeControl.bind(t));

// Connection events
t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
t.addEvent('connection:pong', function(){t.trigger('pong');});
...
```

#### <a name="apidoc.element.monitor._.prototype.bindAll"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>bindAll ()](#apidoc.element.monitor._.prototype.bindAll)
- description and source-code
```javascript
bindAll = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.chain"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>chain ()](#apidoc.element.monitor._.prototype.chain)
- description and source-code
```javascript
chain = function () {
  this._chain = true;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.clone"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>clone ()](#apidoc.element.monitor._.prototype.clone)
- description and source-code
```javascript
clone = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
        var onConnect = function(error, probe) {
if (error) {return callback(error);}
probeJSON = probe.toJSON();
probeJSON.probeId = probeJSON.id; delete probeJSON.id;
monitor.probe = probe;

// Keep the last known probe state for effective updating
monitor._probeValues = _.clone(probeJSON);

// Perform the initial set silently.  This assures the initial
// probe contents are available on the connect event,
// but doesn't fire a change event before connect.
monitor.set(probeJSON, {silent:true});

// Watch the probe for changes.
...
```

#### <a name="apidoc.element.monitor._.prototype.collect"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>collect ()](#apidoc.element.monitor._.prototype.collect)
- description and source-code
```javascript
collect = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.compact"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>compact ()](#apidoc.element.monitor._.prototype.compact)
- description and source-code
```javascript
compact = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.compose"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>compose ()](#apidoc.element.monitor._.prototype.compose)
- description and source-code
```javascript
compose = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.concat"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>concat ()](#apidoc.element.monitor._.prototype.concat)
- description and source-code
```javascript
concat = function () {
  return result.call(this, method.apply(this._wrapped, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.contains"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>contains ()](#apidoc.element.monitor._.prototype.contains)
- description and source-code
```javascript
contains = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.countBy"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>countBy ()](#apidoc.element.monitor._.prototype.countBy)
- description and source-code
```javascript
countBy = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.debounce"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>debounce ()](#apidoc.element.monitor._.prototype.debounce)
- description and source-code
```javascript
debounce = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.defaults"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>defaults ()](#apidoc.element.monitor._.prototype.defaults)
- description and source-code
```javascript
defaults = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.defer"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>defer ()](#apidoc.element.monitor._.prototype.defer)
- description and source-code
```javascript
defer = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.delay"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>delay ()](#apidoc.element.monitor._.prototype.delay)
- description and source-code
```javascript
delay = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.detect"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>detect ()](#apidoc.element.monitor._.prototype.detect)
- description and source-code
```javascript
detect = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.difference"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>difference ()](#apidoc.element.monitor._.prototype.difference)
- description and source-code
```javascript
difference = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.drop"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>drop ()](#apidoc.element.monitor._.prototype.drop)
- description and source-code
```javascript
drop = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.each"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>each ()](#apidoc.element.monitor._.prototype.each)
- description and source-code
```javascript
each = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
  t.addHostCallbacks[hostName].forEach(function(cb) {
    cb(error);
  });
  delete t.addHostCallbacks[hostName];
};

// Build the list of ports already connected
t.connections.each(function(connection){
  var host = connection.get('hostName').toLowerCase();
  var port = connection.get('hostPort');
  if (host === hostName && port >= portStart && port <= portEnd) {
    connectedPorts.push(port);
  }
});
...
```

#### <a name="apidoc.element.monitor._.prototype.escape"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>escape ()](#apidoc.element.monitor._.prototype.escape)
- description and source-code
```javascript
escape = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.every"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>every ()](#apidoc.element.monitor._.prototype.every)
- description and source-code
```javascript
every = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.extend"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>extend ()](#apidoc.element.monitor._.prototype.extend)
- description and source-code
```javascript
extend = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
  * Connected to remote monitor process
  *
  * This event is emitted after the two sides of the connection have exchanged
  * information about themselves.
  *
  * @event connect
  */
  var Connection = Monitor.Connection = Backbone.Model.extend({

defaults:  {
  hostName: '',
  hostPort: null,
  url: null,
  socket: null,
  gateway: false,
...
```

#### <a name="apidoc.element.monitor._.prototype.filter"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>filter ()](#apidoc.element.monitor._.prototype.filter)
- description and source-code
```javascript
filter = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
    * @protected
    * @param hostName {String} - Host name to search for (null = any host)
    * @param appName {String} - App name to search for (null = any app)
    * @return connections {Array of Connection} - An array of Connection objects matching the criteria
    */
    findConnections: function(hostName, appName) {
      var t = this;
      return t.connections.filter(function(conn) {

// Host or app matches if not specified or if specified and equal
var matchesHost = !hostName || conn.isThisHost(hostName);
var matchesApp = !appName || appName === conn.get('remoteAppName');
var remoteFirewall = conn.get('remoteFirewall');

// This is a match if host + app matches, and it's not firewalled
...
```

#### <a name="apidoc.element.monitor._.prototype.find"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>find ()](#apidoc.element.monitor._.prototype.find)
- description and source-code
```javascript
find = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
if (t.runningProbesByKey[probeName] || Probe.classes[probeClass] != null) {
  return callback(null, null);
}

// Give named auto-start probes time to start up
var autoStarts = Monitor.Config.Monitor.autoStart;
if (probeName && !probeClass && autoStarts.length) {
  var autoStart = Monitor._.find(autoStarts, function(probeDef) {
    return probeDef.probeName === probeName;
  });
  if (autoStart) {
    setTimeout(function() {
      t.determineConnection(monitorJSON, makeNewConnections, callback);
    },10);
    return;
...
```

#### <a name="apidoc.element.monitor._.prototype.findWhere"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>findWhere ()](#apidoc.element.monitor._.prototype.findWhere)
- description and source-code
```javascript
findWhere = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.first"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>first ()](#apidoc.element.monitor._.prototype.first)
- description and source-code
```javascript
first = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.flatten"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>flatten ()](#apidoc.element.monitor._.prototype.flatten)
- description and source-code
```javascript
flatten = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.foldl"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>foldl ()](#apidoc.element.monitor._.prototype.foldl)
- description and source-code
```javascript
foldl = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.foldr"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>foldr ()](#apidoc.element.monitor._.prototype.foldr)
- description and source-code
```javascript
foldr = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.forEach"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>forEach ()](#apidoc.element.monitor._.prototype.forEach)
- description and source-code
```javascript
forEach = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...

  // Allow probes to be externally identified by name
  if (probeJSON.probeName) {
    return probeJSON.probeName;
  }

  if (initParams) {
    _.keys(initParams).sort().forEach(function(key){
      probeKey += ':' + key + '=' + initParams[key];
    });
  }
  return probeKey;
},

/**
...
```

#### <a name="apidoc.element.monitor._.prototype.functions"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>functions ()](#apidoc.element.monitor._.prototype.functions)
- description and source-code
```javascript
functions = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.groupBy"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>groupBy ()](#apidoc.element.monitor._.prototype.groupBy)
- description and source-code
```javascript
groupBy = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.has"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>has ()](#apidoc.element.monitor._.prototype.has)
- description and source-code
```javascript
has = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...

// Cannot liveSync with a collection (too many issues)
if (options.liveSync && model instanceof Backbone.Collection) {
  return options.error(null, 'Cannot liveSync with a collection');
}

// Generate an ID if necessary
if (!model.has('id')) {
  if (method === METHOD_CREATE) {
    model.set({id: Monitor.generateUniqueId()}, {silent: true});
    logger.info('_sync.generateUniqueId', t.className, model.toJSON(), options);
  } else {
    return options.error(null, 'ID element must be set.');
  }
}
...
```

#### <a name="apidoc.element.monitor._.prototype.head"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>head ()](#apidoc.element.monitor._.prototype.head)
- description and source-code
```javascript
head = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.identity"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>identity ()](#apidoc.element.monitor._.prototype.identity)
- description and source-code
```javascript
identity = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.include"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>include ()](#apidoc.element.monitor._.prototype.include)
- description and source-code
```javascript
include = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>indexOf ()](#apidoc.element.monitor._.prototype.indexOf)
- description and source-code
```javascript
indexOf = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
    set_control: function(attrs, callback) {
var t = this,
    writableAttributes = t.get('writableAttributes') || [];

// Validate the attributes are writable
if (writableAttributes !== '*') {
  for (var attrName in attrs) {
    if (writableAttributes.indexOf(attrName) < 0) {
      return callback({code:'NOT_WRITABLE', msg: 'Attribute not writable: ' + attrName});
    }
  }
}

// Set the data
var error = null;
...
```

#### <a name="apidoc.element.monitor._.prototype.initial"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>initial ()](#apidoc.element.monitor._.prototype.initial)
- description and source-code
```javascript
initial = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.inject"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>inject ()](#apidoc.element.monitor._.prototype.inject)
- description and source-code
```javascript
inject = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.intersection"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>intersection ()](#apidoc.element.monitor._.prototype.intersection)
- description and source-code
```javascript
intersection = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.invert"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>invert ()](#apidoc.element.monitor._.prototype.invert)
- description and source-code
```javascript
invert = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.invoke"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>invoke ()](#apidoc.element.monitor._.prototype.invoke)
- description and source-code
```javascript
invoke = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isArguments"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isArguments ()](#apidoc.element.monitor._.prototype.isArguments)
- description and source-code
```javascript
isArguments = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isArray"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isArray ()](#apidoc.element.monitor._.prototype.isArray)
- description and source-code
```javascript
isArray = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isBoolean"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isBoolean ()](#apidoc.element.monitor._.prototype.isBoolean)
- description and source-code
```javascript
isBoolean = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isDate"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isDate ()](#apidoc.element.monitor._.prototype.isDate)
- description and source-code
```javascript
isDate = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isElement"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isElement ()](#apidoc.element.monitor._.prototype.isElement)
- description and source-code
```javascript
isElement = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isEmpty ()](#apidoc.element.monitor._.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isEqual"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isEqual ()](#apidoc.element.monitor._.prototype.isEqual)
- description and source-code
```javascript
isEqual = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
      };

      // Client-side listener - for persisting changes to the server
      var modelListener = function(changedModel, options) {
options = options || {};

// Don't persist unless the model is different
if (_.isEqual(JSON.parse(JSON.stringify(model)), JSON.parse(JSON.stringify(model.syncMonitor.get('model'))))) {
  logger.info('modelListener.noChanges', t.className, model.toJSON());
  return;
}

// Disconnect listeners if the ID changes
if (model.get('id') !== modelId) {
  logger.info('modelListener.alteredId', t.className, model.toJSON());
...
```

#### <a name="apidoc.element.monitor._.prototype.isFinite"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isFinite ()](#apidoc.element.monitor._.prototype.isFinite)
- description and source-code
```javascript
isFinite = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isFunction"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isFunction ()](#apidoc.element.monitor._.prototype.isFunction)
- description and source-code
```javascript
isFunction = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isNaN"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isNaN ()](#apidoc.element.monitor._.prototype.isNaN)
- description and source-code
```javascript
isNaN = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isNull"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isNull ()](#apidoc.element.monitor._.prototype.isNull)
- description and source-code
```javascript
isNull = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isNumber"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isNumber ()](#apidoc.element.monitor._.prototype.isNumber)
- description and source-code
```javascript
isNumber = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
* for maintaining the prior and new value for the stat.
*
* @method increment
* @param name {String} Dot.separated name of the counter to increment
* @param [value=1] {Number} Amount to increment the counter by.
*/
proto.increment = function(name, value){
  value = _.isNumber(value) ? value : 1;
  Stat._emit(this.module, name, value, 'c');
};

/**
* Decrement a counter by a specified value
*
* Assuming someone is listening to this stat, this is an instruction for that
...
```

#### <a name="apidoc.element.monitor._.prototype.isObject"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isObject ()](#apidoc.element.monitor._.prototype.isObject)
- description and source-code
```javascript
isObject = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isRegExp"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isRegExp ()](#apidoc.element.monitor._.prototype.isRegExp)
- description and source-code
```javascript
isRegExp = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isString"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isString ()](#apidoc.element.monitor._.prototype.isString)
- description and source-code
```javascript
isString = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.isUndefined"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>isUndefined ()](#apidoc.element.monitor._.prototype.isUndefined)
- description and source-code
```javascript
isUndefined = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
    * @return connection {Connection} - The added connection
    */
    addConnection: function(options) {
var t = this,
    startTime = Date.now();

// Default the firewall value
if (_.isUndefined(options.firewall)) {
  options = _.extend({},options, {firewall: t.firewall});
}

// Generate a unique ID for the connection
options.id = Monitor.generateUniqueCollectionId(t.connections);

var connStr = 'Conn_' + options.id;
...
```

#### <a name="apidoc.element.monitor._.prototype.join"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>join ()](#apidoc.element.monitor._.prototype.join)
- description and source-code
```javascript
join = function () {
  return result.call(this, method.apply(this._wrapped, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.keys"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>keys ()](#apidoc.element.monitor._.prototype.keys)
- description and source-code
```javascript
keys = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...

  // Exchange connection information
  socket.emit('connection:info', {
    hostName:Monitor.getRouter().getHostName(),
    appName:Config.Monitor.appName,
    appInstance: appInstance,
    pid: pid,
    probeClasses: _.keys(Probe.classes),
    gateway:t.get('gateway'),
    firewall:t.get('firewall')
  });
},

/**
* Process an inbound request to connect with a probe
...
```

#### <a name="apidoc.element.monitor._.prototype.last"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>last ()](#apidoc.element.monitor._.prototype.last)
- description and source-code
```javascript
last = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>lastIndexOf ()](#apidoc.element.monitor._.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.map"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>map ()](#apidoc.element.monitor._.prototype.map)
- description and source-code
```javascript
map = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.max"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>max ()](#apidoc.element.monitor._.prototype.max)
- description and source-code
```javascript
max = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.memoize"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>memoize ()](#apidoc.element.monitor._.prototype.memoize)
- description and source-code
```javascript
memoize = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.methods"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>methods ()](#apidoc.element.monitor._.prototype.methods)
- description and source-code
```javascript
methods = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.min"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>min ()](#apidoc.element.monitor._.prototype.min)
- description and source-code
```javascript
min = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.mixin"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>mixin ()](#apidoc.element.monitor._.prototype.mixin)
- description and source-code
```javascript
mixin = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.noConflict"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>noConflict ()](#apidoc.element.monitor._.prototype.noConflict)
- description and source-code
```javascript
noConflict = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.object"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>object ()](#apidoc.element.monitor._.prototype.object)
- description and source-code
```javascript
object = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.omit"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>omit ()](#apidoc.element.monitor._.prototype.omit)
- description and source-code
```javascript
omit = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.once"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>once ()](#apidoc.element.monitor._.prototype.once)
- description and source-code
```javascript
once = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.pairs"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>pairs ()](#apidoc.element.monitor._.prototype.pairs)
- description and source-code
```javascript
pairs = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.partial"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>partial ()](#apidoc.element.monitor._.prototype.partial)
- description and source-code
```javascript
partial = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.pick"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>pick ()](#apidoc.element.monitor._.prototype.pick)
- description and source-code
```javascript
pick = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
  *   params for the class.
  * @return {Object} The monitor parameters
  */
  Sync.prototype._getMonitorParams = function(modelId) {

// Build server connection parameters from this instance of Sync
var t = this;
var params = _.pick(t.options, 'hostName', 'appName', 'appInstance');

// Add probe and class parameters
params.probeClass = 'Sync';
params.initParams = {
  className: t.className
};
...
```

#### <a name="apidoc.element.monitor._.prototype.pluck"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>pluck ()](#apidoc.element.monitor._.prototype.pluck)
- description and source-code
```javascript
pluck = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.pop"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>pop ()](#apidoc.element.monitor._.prototype.pop)
- description and source-code
```javascript
pop = function () {
  var obj = this._wrapped;
  method.apply(obj, arguments);
  if ((name == 'shift' || name == 'splice') && obj.length === 0) delete obj[0];
  return result.call(this, obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.push"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>push ()](#apidoc.element.monitor._.prototype.push)
- description and source-code
```javascript
push = function () {
  var obj = this._wrapped;
  method.apply(obj, arguments);
  if ((name == 'shift' || name == 'splice') && obj.length === 0) delete obj[0];
  return result.call(this, obj);
}
```
- example usage
```shell
...

// Create an array to hold callbacks for this host
if (!t.addHostCallbacks[hostName]) {
  t.addHostCallbacks[hostName] = [];
}

// Remember this callback and return if we're already adding connections for this host
if (t.addHostCallbacks[hostName].push(callback) > 1) {
  return;
}

// Called when done
var doneAdding = function(error) {
  t.addHostCallbacks[hostName].forEach(function(cb) {
    cb(error);
...
```

#### <a name="apidoc.element.monitor._.prototype.random"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>random ()](#apidoc.element.monitor._.prototype.random)
- description and source-code
```javascript
random = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.range"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>range ()](#apidoc.element.monitor._.prototype.range)
- description and source-code
```javascript
range = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.reduce"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>reduce ()](#apidoc.element.monitor._.prototype.reduce)
- description and source-code
```javascript
reduce = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>reduceRight ()](#apidoc.element.monitor._.prototype.reduceRight)
- description and source-code
```javascript
reduceRight = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.reject"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>reject ()](#apidoc.element.monitor._.prototype.reject)
- description and source-code
```javascript
reject = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.rest"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>rest ()](#apidoc.element.monitor._.prototype.rest)
- description and source-code
```javascript
rest = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.result"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>result ()](#apidoc.element.monitor._.prototype.result)
- description and source-code
```javascript
result = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.reverse"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>reverse ()](#apidoc.element.monitor._.prototype.reverse)
- description and source-code
```javascript
reverse = function () {
  var obj = this._wrapped;
  method.apply(obj, arguments);
  if ((name == 'shift' || name == 'splice') && obj.length === 0) delete obj[0];
  return result.call(this, obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.select"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>select ()](#apidoc.element.monitor._.prototype.select)
- description and source-code
```javascript
select = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.shift"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>shift ()](#apidoc.element.monitor._.prototype.shift)
- description and source-code
```javascript
shift = function () {
  var obj = this._wrapped;
  method.apply(obj, arguments);
  if ((name == 'shift' || name == 'splice') && obj.length === 0) delete obj[0];
  return result.call(this, obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.shuffle"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>shuffle ()](#apidoc.element.monitor._.prototype.shuffle)
- description and source-code
```javascript
shuffle = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.size"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>size ()](#apidoc.element.monitor._.prototype.size)
- description and source-code
```javascript
size = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
...
var newModel = model.syncMonitor.get('model');
if (_.isEqual(JSON.parse(JSON.stringify(model)), JSON.parse(JSON.stringify(newModel)))) {
  logger.info('monitorListener.noChanges', t.className, newModel);
  return;
}

// Disconnect if the model was deleted or the ID isn't the same
var isDeleted = (_.size(newModel) === 0);
if (isDeleted || newModel.id !== modelId)  {
  logger.info('modelListener.deleted', t.className, newModel);
  disconnectListeners();
}

// Forward changes to the model (including server-side delete)
var newOpts = {isSyncChanging:true};
...
```

#### <a name="apidoc.element.monitor._.prototype.slice"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>slice ()](#apidoc.element.monitor._.prototype.slice)
- description and source-code
```javascript
slice = function () {
  return result.call(this, method.apply(this._wrapped, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.some"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>some ()](#apidoc.element.monitor._.prototype.some)
- description and source-code
```javascript
some = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.sort"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>sort ()](#apidoc.element.monitor._.prototype.sort)
- description and source-code
```javascript
sort = function () {
  var obj = this._wrapped;
  method.apply(obj, arguments);
  if ((name == 'shift' || name == 'splice') && obj.length === 0) delete obj[0];
  return result.call(this, obj);
}
```
- example usage
```shell
...

  // Allow probes to be externally identified by name
  if (probeJSON.probeName) {
    return probeJSON.probeName;
  }

  if (initParams) {
    _.keys(initParams).sort().forEach(function(key){
      probeKey += ':' + key + '=' + initParams[key];
    });
  }
  return probeKey;
},

/**
...
```

#### <a name="apidoc.element.monitor._.prototype.sortBy"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>sortBy ()](#apidoc.element.monitor._.prototype.sortBy)
- description and source-code
```javascript
sortBy = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.sortedIndex"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>sortedIndex ()](#apidoc.element.monitor._.prototype.sortedIndex)
- description and source-code
```javascript
sortedIndex = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.splice"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>splice ()](#apidoc.element.monitor._.prototype.splice)
- description and source-code
```javascript
splice = function () {
  var obj = this._wrapped;
  method.apply(obj, arguments);
  if ((name == 'shift' || name == 'splice') && obj.length === 0) delete obj[0];
  return result.call(this, obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.tail"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>tail ()](#apidoc.element.monitor._.prototype.tail)
- description and source-code
```javascript
tail = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.take"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>take ()](#apidoc.element.monitor._.prototype.take)
- description and source-code
```javascript
take = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.tap"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>tap ()](#apidoc.element.monitor._.prototype.tap)
- description and source-code
```javascript
tap = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.template"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>template ()](#apidoc.element.monitor._.prototype.template)
- description and source-code
```javascript
template = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.throttle"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>throttle ()](#apidoc.element.monitor._.prototype.throttle)
- description and source-code
```javascript
throttle = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.times"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>times ()](#apidoc.element.monitor._.prototype.times)
- description and source-code
```javascript
times = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.toArray"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>toArray ()](#apidoc.element.monitor._.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.unescape"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>unescape ()](#apidoc.element.monitor._.prototype.unescape)
- description and source-code
```javascript
unescape = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.union"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>union ()](#apidoc.element.monitor._.prototype.union)
- description and source-code
```javascript
union = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.uniq"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>uniq ()](#apidoc.element.monitor._.prototype.uniq)
- description and source-code
```javascript
uniq = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.unique"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>unique ()](#apidoc.element.monitor._.prototype.unique)
- description and source-code
```javascript
unique = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.uniqueId"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>uniqueId ()](#apidoc.element.monitor._.prototype.uniqueId)
- description and source-code
```javascript
uniqueId = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.unshift"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>unshift ()](#apidoc.element.monitor._.prototype.unshift)
- description and source-code
```javascript
unshift = function () {
  var obj = this._wrapped;
  method.apply(obj, arguments);
  if ((name == 'shift' || name == 'splice') && obj.length === 0) delete obj[0];
  return result.call(this, obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.value"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>value ()](#apidoc.element.monitor._.prototype.value)
- description and source-code
```javascript
value = function () {
  return this._wrapped;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.values"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>values ()](#apidoc.element.monitor._.prototype.values)
- description and source-code
```javascript
values = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.where"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>where ()](#apidoc.element.monitor._.prototype.where)
- description and source-code
```javascript
where = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.without"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>without ()](#apidoc.element.monitor._.prototype.without)
- description and source-code
```javascript
without = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.wrap"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>wrap ()](#apidoc.element.monitor._.prototype.wrap)
- description and source-code
```javascript
wrap = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor._.prototype.zip"></a>[function <span class="apidocSignatureSpan">monitor._.prototype.</span>zip ()](#apidoc.element.monitor._.prototype.zip)
- description and source-code
```javascript
zip = function () {
  var args = [this._wrapped];
  push.apply(args, arguments);
  return result.call(this, func.apply(_, args));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monitor.__super__"></a>[module monitor.__super__](#apidoc.module.monitor.__super__)

#### <a name="apidoc.element.monitor.__super__._computeChanges"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>_computeChanges (loud)](#apidoc.element.monitor.__super__._computeChanges)
- description and source-code
```javascript
_computeChanges = function (loud) {
  this.changed = {};
  var already = {};
  var triggers = [];
  var current = this._currentAttributes;
  var changes = this._changes;

  // Loop through the current queue of potential model changes.
  for (var i = changes.length - 2; i >= 0; i -= 2) {
    var key = changes[i], val = changes[i + 1];
    if (already[key]) continue;
    already[key] = true;

    // Check if the attribute has been modified since the last change,
    // and update 'this.changed' accordingly. If we're inside of a 'change'
    // call, also add a trigger to the list.
    if (current[key] !== val) {
      this.changed[key] = val;
      if (!loud) continue;
      triggers.push(key, val);
      current[key] = val;
    }
  }
  if (loud) this._changes = [];

  // Signals 'this.changed' is current to prevent duplicate calls from 'this.hasChanged'.
  this._hasComputed = true;
  return triggers;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__._validate"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>_validate (attrs, options)](#apidoc.element.monitor.__super__._validate)
- description and source-code
```javascript
_validate = function (attrs, options) {
  if (!this.validate) return true;
  attrs = _.extend({}, this.attributes, attrs);
  var error = this.validate(attrs, options);
  if (!error) return true;
  if (options && options.error) options.error(this, error, options);
  this.trigger('error', this, error, options);
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.bind"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>bind (name, callback, context)](#apidoc.element.monitor.__super__.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
t.addEvent('disconnect', function(){t.disconnect('remote_disconnect');});
t.addEvent('error', function(reason){
  t.trigger('error', reason);
  t.disconnect('connect error');
});

// Inbound probe events
t.addEvent('probe:connect', t.probeConnect.bind(t));
t.addEvent('probe:disconnect', t.probeDisconnect.bind(t));
t.addEvent('probe:control', t.probeControl.bind(t));

// Connection events
t.addEvent('connection:ping', function(){socket.emit('connection:pong');});
t.addEvent('connection:pong', function(){t.trigger('pong');});
...
```

#### <a name="apidoc.element.monitor.__super__.change"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>change (options)](#apidoc.element.monitor.__super__.change)
- description and source-code
```javascript
change = function (options) {
  var changing = this._changing;
  this._changing = true;

  // Generate the changes to be triggered on the model.
  var triggers = this._computeChanges(true);

  this._pending = !!triggers.length;

  for (var i = triggers.length - 2; i >= 0; i -= 2) {
    this.trigger('change:' + triggers[i], this, triggers[i + 1], options);
  }

  if (changing) return this;

  // Trigger a 'change' while there have been changes.
  while (this._pending) {
    this._pending = false;
    this.trigger('change', this, options);
    this._previousAttributes = _.clone(this.attributes);
  }

  this._changing = false;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.changedAttributes"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>changedAttributes (diff)](#apidoc.element.monitor.__super__.changedAttributes)
- description and source-code
```javascript
changedAttributes = function (diff) {
  if (!diff) return this.hasChanged() ? _.clone(this.changed) : false;
  var val, changed = false, old = this._previousAttributes;
  for (var attr in diff) {
    if (_.isEqual(old[attr], (val = diff[attr]))) continue;
    (changed || (changed = {}))[attr] = val;
  }
  return changed;
}
```
- example usage
```shell
...
// Connect the montior proxy
monitorProxy = new Monitor(monitorJSON);
monitorProxy.set('probeId', probeId);
t.incomingMonitorsById[probeId] = monitorProxy;
monitorProxy.probe = probe;
monitorProxy.probeChange = function(){
  try {
    t.emit('probe:change:' + probeId, probe.changedAttributes());
  }
  catch (e) {
    log.error('probeChange', e, probe, logCtxt);
  }
};
probe.connectTime = Date.now();
var duration = probe.connectTime - startTime;
...
```

#### <a name="apidoc.element.monitor.__super__.clear"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>clear (options)](#apidoc.element.monitor.__super__.clear)
- description and source-code
```javascript
clear = function (options) {
  var attrs = {};
  for (var key in this.attributes) attrs[key] = void 0;
  return this.set(attrs, _.extend({}, options, {unset: true}));
}
```
- example usage
```shell
...
*
* Live data synchronization consumes resources on both the client and server.
* To release those resources, make sure to call the '''clear()''' method on
* the data model. Otherwise, resources are released when the server connection
* is terminated.
*
*     // Clear the object, turning off live synchronization
*     myBook.clear();
*
* See the <a href="http://documentcloud.github.com/backbone/#Sync">Backbone documentation</a>
* for more information about the Backbone.sync functionality.
*
* @static
* @method Sync
* @param className {String} Name of the class to synchronize with
...
```

#### <a name="apidoc.element.monitor.__super__.clone"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>clone ()](#apidoc.element.monitor.__super__.clone)
- description and source-code
```javascript
clone = function () {
  return new this.constructor(this.attributes);
}
```
- example usage
```shell
...
        var onConnect = function(error, probe) {
if (error) {return callback(error);}
probeJSON = probe.toJSON();
probeJSON.probeId = probeJSON.id; delete probeJSON.id;
monitor.probe = probe;

// Keep the last known probe state for effective updating
monitor._probeValues = _.clone(probeJSON);

// Perform the initial set silently.  This assures the initial
// probe contents are available on the connect event,
// but doesn't fire a change event before connect.
monitor.set(probeJSON, {silent:true});

// Watch the probe for changes.
...
```

#### <a name="apidoc.element.monitor.__super__.destroy"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>destroy ()](#apidoc.element.monitor.__super__.destroy)
- description and source-code
```javascript
destroy = function () {

  // Connect the success/error methods for callback style requests.
  // These style callbacks don't need the model or options arguments
  // because they're in the scope of the anonymous callback function.
  var args = _.toArray(arguments), callback = args[args.length - 1];
  if (typeof callback === 'function') {

    // Remove the last element (the callback)
    args.splice(-1, 1);

    // Place options if none were specified.
    if (args.length === 0) {
      args.push({});
    }

    // Place attributes if save and only options were specified
    if (args.length === 1 && methodName === 'save') {
      args.push({});
    }
    var options = args[args.length - 1];

    // Place the success and error methods
    options.success = function(model, response) {
      callback(null, response);
    };
    options.error = function(model, response) {
      // Provide the response as the error.
      callback(response, null);
    };
  }

  // Invoke the original method
  return method.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.escape"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>escape (attr)](#apidoc.element.monitor.__super__.escape)
- description and source-code
```javascript
escape = function (attr) {
  return _.escape(this.get(attr));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.fetch"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>fetch ()](#apidoc.element.monitor.__super__.fetch)
- description and source-code
```javascript
fetch = function () {

  // Connect the success/error methods for callback style requests.
  // These style callbacks don't need the model or options arguments
  // because they're in the scope of the anonymous callback function.
  var args = _.toArray(arguments), callback = args[args.length - 1];
  if (typeof callback === 'function') {

    // Remove the last element (the callback)
    args.splice(-1, 1);

    // Place options if none were specified.
    if (args.length === 0) {
      args.push({});
    }

    // Place attributes if save and only options were specified
    if (args.length === 1 && methodName === 'save') {
      args.push({});
    }
    var options = args[args.length - 1];

    // Place the success and error methods
    options.success = function(model, response) {
      callback(null, response);
    };
    options.error = function(model, response) {
      // Provide the response as the error.
      callback(response, null);
    };
  }

  // Invoke the original method
  return method.apply(this, args);
}
```
- example usage
```shell
...
*       ...
*     });
*
* The sync function can also be assigned to any Backbone model after construction:
*
*     var myBook = new Book({id:"44329"});
*     myBook.sync = Monitor.Sync('Book');
*     myBook.fetch();
*
* In addition to providing the standard '''fetch''', '''save''', and '''destroy'''
* functionality, Sync offers *live data synchronization*, updating the data model
* as changes are detected on the server.
*
*     // Turn on live data synchronization
*     myBook.fetch({liveSync:true});
...
```

#### <a name="apidoc.element.monitor.__super__.get"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>get (attr)](#apidoc.element.monitor.__super__.get)
- description and source-code
```javascript
get = function (attr) {
  return this.attributes[attr];
}
```
- example usage
```shell
...
For this example, we'll monitor the *Process* probe:

    > var processMonitor = new Monitor({probeClass:'Process'});
    > processMonitor.connect();

The monitor is a [Backbone.js](http://backbonejs.org/) data model so it updates in real time, and you can get all fields with toJSON
():

    > processMonitor.get('freemem');
    86368256
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:
...
```

#### <a name="apidoc.element.monitor.__super__.has"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>has (attr)](#apidoc.element.monitor.__super__.has)
- description and source-code
```javascript
has = function (attr) {
  return this.get(attr) != null;
}
```
- example usage
```shell
...

// Cannot liveSync with a collection (too many issues)
if (options.liveSync && model instanceof Backbone.Collection) {
  return options.error(null, 'Cannot liveSync with a collection');
}

// Generate an ID if necessary
if (!model.has('id')) {
  if (method === METHOD_CREATE) {
    model.set({id: Monitor.generateUniqueId()}, {silent: true});
    logger.info('_sync.generateUniqueId', t.className, model.toJSON(), options);
  } else {
    return options.error(null, 'ID element must be set.');
  }
}
...
```

#### <a name="apidoc.element.monitor.__super__.hasChanged"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>hasChanged (attr)](#apidoc.element.monitor.__super__.hasChanged)
- description and source-code
```javascript
hasChanged = function (attr) {
  if (!this._hasComputed) this._computeChanges();
  if (attr == null) return !_.isEmpty(this.changed);
  return _.has(this.changed, attr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.initialize"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>initialize ()](#apidoc.element.monitor.__super__.initialize)
- description and source-code
```javascript
initialize = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.isNew"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>isNew ()](#apidoc.element.monitor.__super__.isNew)
- description and source-code
```javascript
isNew = function () {
  return this.id == null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.listenTo"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>listenTo (object, events, callback)](#apidoc.element.monitor.__super__.listenTo)
- description and source-code
```javascript
listenTo = function (object, events, callback) {
  var listeners = this._listeners || (this._listeners = {});
  var id = object._listenerId || (object._listenerId = _.uniqueId('l'));
  listeners[id] = object;
  object.on(events, callback || this, this);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.off"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>off (name, callback, context)](#apidoc.element.monitor.__super__.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
...
* @method ping
* @param callback {Function(error)} Callback when response is returned
*/
ping: function(callback) {
  var t = this;
  callback = callback || function(){};
  var onPong = function() {
    t.off('pong', onPong);
    callback();
  };
  t.on('pong', onPong);
  t.emit('connection:ping');
},

/**
...
```

#### <a name="apidoc.element.monitor.__super__.on"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>on (name, callback, context)](#apidoc.element.monitor.__super__.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  if (!(eventsApi(this, 'on', name, [callback, context]) && callback)) return this;
  this._events || (this._events = {});
  var list = this._events[name] || (this._events[name] = []);
  list.push({callback: callback, context: context, ctx: context || this});
  return this;
}
```
- example usage
```shell
...
    > processMonitor.get('freemem');
    80044032
    > processMonitor.toJSON();
    ...

As the monitor changes, it emits change events:

    > processMonitor.on('change', function() {
    ... console.log(processMonitor.get('freemem'));
    ... });

Monitoring your app with a custom script
----------------------------------------

Using Node.js as a scripting language, you can write custom monitors that do anything Node.js can do.  Here's an example that prints
 to the console when free memory falls below a threshold.
...
```

#### <a name="apidoc.element.monitor.__super__.once"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>once (name, callback, context)](#apidoc.element.monitor.__super__.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  if (!(eventsApi(this, 'once', name, [callback, context]) && callback)) return this;
  var self = this;
  var once = _.once(function() {
    self.off(name, once);
    callback.apply(this, arguments);
  });
  once._callback = callback;
  this.on(name, once, context);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.parse"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>parse (resp)](#apidoc.element.monitor.__super__.parse)
- description and source-code
```javascript
parse = function (resp) {
  return resp;
}
```
- example usage
```shell
...
      };

      // Client-side listener - for persisting changes to the server
      var modelListener = function(changedModel, options) {
options = options || {};

// Don't persist unless the model is different
if (_.isEqual(JSON.parse(JSON.stringify(model)), JSON.parse(JSON.stringify(model.syncMonitor.get('model'))))) {
  logger.info('modelListener.noChanges', t.className, model.toJSON());
  return;
}

// Disconnect listeners if the ID changes
if (model.get('id') !== modelId) {
  logger.info('modelListener.alteredId', t.className, model.toJSON());
...
```

#### <a name="apidoc.element.monitor.__super__.previous"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>previous (attr)](#apidoc.element.monitor.__super__.previous)
- description and source-code
```javascript
previous = function (attr) {
  if (attr == null || !this._previousAttributes) return null;
  return this._previousAttributes[attr];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.previousAttributes"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>previousAttributes ()](#apidoc.element.monitor.__super__.previousAttributes)
- description and source-code
```javascript
previousAttributes = function () {
  return _.clone(this._previousAttributes);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.save"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>save ()](#apidoc.element.monitor.__super__.save)
- description and source-code
```javascript
save = function () {

  // Connect the success/error methods for callback style requests.
  // These style callbacks don't need the model or options arguments
  // because they're in the scope of the anonymous callback function.
  var args = _.toArray(arguments), callback = args[args.length - 1];
  if (typeof callback === 'function') {

    // Remove the last element (the callback)
    args.splice(-1, 1);

    // Place options if none were specified.
    if (args.length === 0) {
      args.push({});
    }

    // Place attributes if save and only options were specified
    if (args.length === 1 && methodName === 'save') {
      args.push({});
    }
    var options = args[args.length - 1];

    // Place the success and error methods
    options.success = function(model, response) {
      callback(null, response);
    };
    options.error = function(model, response) {
      // Provide the response as the error.
      callback(response, null);
    };
  }

  // Invoke the original method
  return method.apply(this, args);
}
```
- example usage
```shell
...
  logger.info('modelListener.alteredId', t.className, model.toJSON());
  return disconnectListeners();
}

// Persist changes to the server (unless the changes originated from there)
if (!options.isSyncChanging) {
  logger.info('modelListener.saving', t.className, model.toJSON());
  model.save();
}
      };

      // Server-side listener - for updating server changes into the model
      var monitorListener = function(changedModel, options) {

// Don't update unless the model is different
...
```

#### <a name="apidoc.element.monitor.__super__.set"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>set (key, val, options)](#apidoc.element.monitor.__super__.set)
- description and source-code
```javascript
set = function (key, val, options) {
  var attr, attrs;
  if (key == null) return this;

  // Handle both '"key", value' and '{key: value}' -style arguments.
  if (_.isObject(key)) {
    attrs = key;
    options = val;
  } else {
    (attrs = {})[key] = val;
  }

  // Extract attributes and options.
  var silent = options && options.silent;
  var unset = options && options.unset;

  // Run validation.
  if (!this._validate(attrs, options)) return false;

  // Check for changes of 'id'.
  if (this.idAttribute in attrs) this.id = attrs[this.idAttribute];

  var now = this.attributes;

  // For each 'set' attribute...
  for (attr in attrs) {
    val = attrs[attr];

    // Update or delete the current value, and track the change.
    unset ? delete now[attr] : now[attr] = val;
    this._changes.push(attr, val);
  }

  // Signal that the model's state has potentially changed, and we need
  // to recompute the actual changes.
  this._hasComputed = false;

  // Fire the '"change"' events.
  if (!silent) this.change(options);
  return this;
}
```
- example usage
```shell
...
    connect: function() {
var t = this, hostName = t.get('hostName'), hostPort = t.get('hostPort'),
url = t.get('url');

// Build the URL if not specified
if (!url) {
  url = t.attributes.url = 'http://' + hostName + ':' + hostPort;
  t.set('url', url);
}

// Connect with this url
var opts = {
  // 'transports': ['websocket', 'xhr-polling', 'jsonp-polling'],
  'force new connection': true,      // Don't re-use existing connections
  'reconnect': false                 // Don't let socket.io reconnect.
...
```

#### <a name="apidoc.element.monitor.__super__.stopListening"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>stopListening (object, events, callback)](#apidoc.element.monitor.__super__.stopListening)
- description and source-code
```javascript
stopListening = function (object, events, callback) {
  var listeners = this._listeners;
  if (!listeners) return;
  if (object) {
    object.off(events, callback, this);
    if (!events && !callback) delete listeners[object._listenerId];
  } else {
    for (var id in listeners) {
      listeners[id].off(null, null, this);
    }
    this._listeners = {};
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.sync"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>sync ()](#apidoc.element.monitor.__super__.sync)
- description and source-code
```javascript
sync = function () {
  return Backbone.sync.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.toJSON"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>toJSON (options)](#apidoc.element.monitor.__super__.toJSON)
- description and source-code
```javascript
toJSON = function (options) {
  return _.clone(this.attributes);
}
```
- example usage
```shell
...

The monitor is a [Backbone.js](http://backbonejs.org/) data model so it updates in real time, and you can get all fields with toJSON
():

> processMonitor.get('freemem');
86368256
> processMonitor.get('freemem');
80044032
> processMonitor.toJSON();
...

As the monitor changes, it emits change events:

> processMonitor.on('change', function() {
... console.log(processMonitor.get('freemem'));
... });
...
```

#### <a name="apidoc.element.monitor.__super__.trigger"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>trigger (name)](#apidoc.element.monitor.__super__.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;
  var args = slice.call(arguments, 1);
  if (!eventsApi(this, 'trigger', name, args)) return this;
  var events = this._events[name];
  var allEvents = this._events.all;
  if (events) triggerEvents(this, events, args);
  if (allEvents) triggerEvents(this, allEvents, arguments);
  return this;
}
```
- example usage
```shell
...

  // Only disconnect once.
  // This method can be called many times during a disconnect (manually,
  // by socketIO disconnect, and/or by the underlying socket disconnect).
  if (t.socketEvents) {
    t.removeAllEvents();
    socket.disconnect();
    t.trigger('disconnect', reason);
    log.info(t.logId + 'disconnect', reason);
  }
},

/**
* Is this connection with the specified host?
*
...
```

#### <a name="apidoc.element.monitor.__super__.unbind"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>unbind (name, callback, context)](#apidoc.element.monitor.__super__.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  var list, ev, events, names, i, l, j, k;
  if (!this._events || !eventsApi(this, 'off', name, [callback, context])) return this;
  if (!name && !callback && !context) {
    this._events = {};
    return this;
  }

  names = name ? [name] : _.keys(this._events);
  for (i = 0, l = names.length; i < l; i++) {
    name = names[i];
    if (list = this._events[name]) {
      events = [];
      if (callback || context) {
        for (j = 0, k = list.length; j < k; j++) {
          ev = list[j];
          if ((callback && callback !== (ev.callback._callback || ev.callback)) ||
              (context && context !== ev.context)) {
            events.push(ev);
          }
        }
      }
      this._events[name] = events;
    }
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.unset"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>unset (attr, options)](#apidoc.element.monitor.__super__.unset)
- description and source-code
```javascript
unset = function (attr, options) {
  return this.set(attr, void 0, _.extend({}, options, {unset: true}));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monitor.__super__.url"></a>[function <span class="apidocSignatureSpan">monitor.__super__.</span>url ()](#apidoc.element.monitor.__super__.url)
- description and source-code
```javascript
url = function () {
  var base = _.result(this, 'urlRoot') || _.result(this.collection, 'url') || urlError();
  if (this.isNew()) return base;
  return base + (base.charAt(base.length - 1) === '/' ? '' : '/') + encodeURIComponent(this.id);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
