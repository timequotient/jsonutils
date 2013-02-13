jsonutils
=========

Converter for JSON data to a Go struct or a Java class for GSON

	b := []byte(`{"Name":"Wednesday","Age":6,"Parents":["Gomez","Morticia"]}`)

	f, err := jsonutils.ParseJson(b)
	if err != nil {
		log.Fatal(err)
	}
	jsonutils.PrintGo(f)