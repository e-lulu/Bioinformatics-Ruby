DATA=???[VDJ].fa IGK-INTRON.fa IGK-KDE.fa TRDD2_upstream.fa TRDD3_downstream.fa ???[VDJ]_upstream.fa ???[VDJ]_downstream.fa

germline:
	sh get-saved-germline

../browser/js/germline.js: $(DATA) germlines.data
	python buildBrowserGermline.py $^ $@

get-all-data:
	sh get-germline
	$(MAKE) ../browser/js/germline.js

clean:
	rm -f $(DATA)
